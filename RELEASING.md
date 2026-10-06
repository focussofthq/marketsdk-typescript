# Releasing

Publishing is by hand, from a clean clone at the tag. The version in `package.json` is stamped by the
generator; nothing here is edited.

One-time setup: an npm account that is a member of the `marketsdk` organization, with two-factor
authentication on.

```bash
npm install -g pnpm@10
pnpm install
pnpm build
npm publish --access public
```

Then check `npm view @marketsdk/js version`.
