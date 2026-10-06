# Reference
## Marketplace
<details><summary><code>client.marketplace.<a href="/src/api/resources/marketplace/client/Client.ts">getMarketplace</a>() -> MarketSDKApi.MarketplaceObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Settings are changed in the dashboard, separately for test and live.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.marketplace.getMarketplace();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**requestOptions:** `MarketplaceClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Sellers
<details><summary><code>client.sellers.<a href="/src/api/resources/sellers/client/Client.ts">listSellers</a>({ ...params }) -> MarketSDKApi.SellerList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.sellers.listSellers();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListSellersRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `SellersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="/src/api/resources/sellers/client/Client.ts">createSeller</a>({ ...params }) -> MarketSDKApi.SellerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.sellers.createSeller({
    external_id: "external_id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreatePartyDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `SellersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="/src/api/resources/sellers/client/Client.ts">getSeller</a>({ ...params }) -> MarketSDKApi.SellerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.sellers.getSeller({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetSellerRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `SellersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="/src/api/resources/sellers/client/Client.ts">eraseSeller</a>({ ...params }) -> MarketSDKApi.SellerObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Removes the name, external id, metadata, storefront, and review text, and takes the listings down. Orders and reputation stay, without personal data.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.sellers.eraseSeller({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.EraseSellerRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `SellersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="/src/api/resources/sellers/client/Client.ts">updateSeller</a>({ ...params }) -> MarketSDKApi.SellerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.sellers.updateSeller({
    id: "id",
    body: {}
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.UpdateSellerRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `SellersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="/src/api/resources/sellers/client/Client.ts">putStorefront</a>({ ...params }) -> MarketSDKApi.StorefrontObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.sellers.putStorefront({
    id: "id",
    name: "name",
    slug: "jane-templates"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.StorefrontDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `SellersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="/src/api/resources/sellers/client/Client.ts">createOnboardingLink</a>({ ...params }) -> MarketSDKApi.OnboardingLinkObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The first link creates the seller's connected account on your Stripe account: Express, with Stripe collecting what the law requires, your platform paying Stripe's fees and bearing losses, and only transfers requested. Send the seller to the link; their payouts status follows as Stripe reports it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.sellers.createOnboardingLink({
    id: "id",
    return_url: "return_url",
    refresh_url: "refresh_url"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.OnboardingLinkDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `SellersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="/src/api/resources/sellers/client/Client.ts">getSellerProfile</a>({ ...params }) -> MarketSDKApi.SellerProfileObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Callable with a publishable key. Shows only what a buyer may see.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.sellers.getSellerProfile({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetSellerProfileRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `SellersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Buyers
<details><summary><code>client.buyers.<a href="/src/api/resources/buyers/client/Client.ts">listBuyers</a>({ ...params }) -> MarketSDKApi.BuyerList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.buyers.listBuyers();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListBuyersRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `BuyersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.buyers.<a href="/src/api/resources/buyers/client/Client.ts">createBuyer</a>({ ...params }) -> MarketSDKApi.BuyerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.buyers.createBuyer({
    external_id: "external_id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreatePartyDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `BuyersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.buyers.<a href="/src/api/resources/buyers/client/Client.ts">getBuyer</a>({ ...params }) -> MarketSDKApi.BuyerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.buyers.getBuyer({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetBuyerRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `BuyersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.buyers.<a href="/src/api/resources/buyers/client/Client.ts">eraseBuyer</a>({ ...params }) -> MarketSDKApi.BuyerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.buyers.eraseBuyer({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.EraseBuyerRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `BuyersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.buyers.<a href="/src/api/resources/buyers/client/Client.ts">updateBuyer</a>({ ...params }) -> MarketSDKApi.BuyerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.buyers.updateBuyer({
    id: "id",
    body: {}
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.UpdateBuyerRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `BuyersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Categories
<details><summary><code>client.categories.<a href="/src/api/resources/categories/client/Client.ts">listCategories</a>({ ...params }) -> MarketSDKApi.CategoryList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.categories.listCategories();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListCategoriesRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `CategoriesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="/src/api/resources/categories/client/Client.ts">createCategory</a>({ ...params }) -> MarketSDKApi.CategoryObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.categories.createCategory({
    key: "ui-kits",
    name: "name"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateCategoryDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `CategoriesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="/src/api/resources/categories/client/Client.ts">getCategory</a>({ ...params }) -> MarketSDKApi.CategoryObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.categories.getCategory({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetCategoryRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `CategoriesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="/src/api/resources/categories/client/Client.ts">updateCategory</a>({ ...params }) -> MarketSDKApi.CategoryObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.categories.updateCategory({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.UpdateCategoryDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `CategoriesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="/src/api/resources/categories/client/Client.ts">getAttributeSchema</a>({ ...params }) -> MarketSDKApi.AttributeSchemaObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.categories.getAttributeSchema({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetAttributeSchemaRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `CategoriesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="/src/api/resources/categories/client/Client.ts">putAttributeSchema</a>({ ...params }) -> MarketSDKApi.AttributeSchemaObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Refused if a listing already in the category would no longer fit.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.categories.putAttributeSchema({
    id: "id",
    body: {
        attributes: [{
                key: "format",
                type: "string"
            }]
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.PutAttributeSchemaRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `CategoriesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Listings
<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">listListings</a>({ ...params }) -> MarketSDKApi.ListingList</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

With a publishable key, only published listings are listed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.listListings();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListListingsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">createListing</a>({ ...params }) -> MarketSDKApi.ListingObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.createListing({
    seller: "sel_034XtPDs7UJ0TXzTsdaHZa",
    title: "title",
    price: {
        amount: 4900,
        currency: "USD"
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateListingDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">createListings</a>({ ...params }) -> MarketSDKApi.BulkListingsObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.createListings({
    listings: [{
            seller: "sel_034XtPDs7UJ0TXzTsdaHZa",
            title: "title",
            price: {
                amount: 4900,
                currency: "USD"
            }
        }]
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.BulkCreateListingsDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">getListing</a>({ ...params }) -> MarketSDKApi.ListingObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

With a publishable key, only a published listing can be retrieved.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.getListing({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetListingRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">updateListing</a>({ ...params }) -> MarketSDKApi.ListingObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.updateListing({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.UpdateListingDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">publishListing</a>({ ...params }) -> MarketSDKApi.ListingObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Needs an active seller, verified when seller verification is on, and a category that is not prohibited.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.publishListing({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.PublishListingRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">unpublishListing</a>({ ...params }) -> MarketSDKApi.ListingObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.unpublishListing({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.UnpublishListingRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">removeListing</a>({ ...params }) -> MarketSDKApi.ListingObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.removeListing({
    id: "id",
    reason: "reason"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.RemoveListingDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">listMedia</a>({ ...params }) -> MarketSDKApi.MediaList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.listMedia({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListMediaRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">createMedia</a>({ ...params }) -> MarketSDKApi.MediaUploadObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns a signed URL, valid for 10 minutes. PUT the file there, then complete the upload. The file is stored under a path that begins with the marketplace id.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.createMedia({
    id: "id",
    content_type: "image/jpeg",
    size_bytes: 1.1
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateMediaDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">completeMedia</a>({ ...params }) -> MarketSDKApi.MediaObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Checks the stored file against the declared type and size.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.completeMedia({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CompleteMediaRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="/src/api/resources/listings/client/Client.ts">deleteMedia</a>({ ...params }) -> MarketSDKApi.MediaObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.listings.deleteMedia({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.DeleteMediaRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ListingsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Search
<details><summary><code>client.search.<a href="/src/api/resources/search/client/Client.ts">searchListings</a>({ ...params }) -> MarketSDKApi.ListingList</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Full text over title and description, with filters and sorting. Only published listings with something available are returned. Callable with a publishable key.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.search.searchListings();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.SearchListingsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `SearchClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Orders
<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">listOrders</a>({ ...params }) -> MarketSDKApi.OrderList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.listOrders();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListOrdersRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">createOrder</a>({ ...params }) -> MarketSDKApi.OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The buyer commits to buy. Quantity is reserved at once. With payments off the order is committed; with payments on it awaits payment.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.createOrder({
    listing: "lst_034XtPDs7UJ0TXzTsdaHZa",
    buyer: "buy_034XtPDs7UJ0TXzTsdaHZa"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateOrderDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">getOrder</a>({ ...params }) -> MarketSDKApi.OrderObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.getOrder({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetOrderRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">listOrderEvents</a>({ ...params }) -> MarketSDKApi.OrderEventList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.listOrderEvents({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListOrderEventsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">claimOrder</a>({ ...params }) -> MarketSDKApi.OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.claimOrder({
    id: "id",
    body: {
        actor: "buy_034XtPDs7UJ0TXzTsdaHZa"
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ClaimOrderRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">confirmOrder</a>({ ...params }) -> MarketSDKApi.OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.confirmOrder({
    id: "id",
    body: {
        actor: "buy_034XtPDs7UJ0TXzTsdaHZa"
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ConfirmOrderRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">backOutOfOrder</a>({ ...params }) -> MarketSDKApi.OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition. Writes a backed_out reputation event against the actor.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.backOutOfOrder({
    id: "id",
    body: {
        actor: "buy_034XtPDs7UJ0TXzTsdaHZa"
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.BackOutOfOrderRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">proposeCancel</a>({ ...params }) -> MarketSDKApi.OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition. The other party can accept within the agreement window. A declined or lapsed proposal changes nothing.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.proposeCancel({
    id: "id",
    body: {
        actor: "buy_034XtPDs7UJ0TXzTsdaHZa"
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ProposeCancelRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">acceptCancel</a>({ ...params }) -> MarketSDKApi.OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.acceptCancel({
    id: "id",
    body: {
        actor: "buy_034XtPDs7UJ0TXzTsdaHZa"
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.AcceptCancelRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">declineCancel</a>({ ...params }) -> MarketSDKApi.OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.declineCancel({
    id: "id",
    body: {
        actor: "buy_034XtPDs7UJ0TXzTsdaHZa"
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.DeclineCancelRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">listOrderReviews</a>({ ...params }) -> MarketSDKApi.ReviewList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.listOrderReviews({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListOrderReviewsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="/src/api/resources/orders/client/Client.ts">createReview</a>({ ...params }) -> MarketSDKApi.ReviewObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition. Only on a completed order, inside the review window, once per party. Hidden until both have reviewed or the window closes.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.orders.createReview({
    id: "id",
    actor: "buy_034XtPDs7UJ0TXzTsdaHZa",
    rating: 1.1
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateReviewDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OrdersClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Reviews
<details><summary><code>client.reviews.<a href="/src/api/resources/reviews/client/Client.ts">listReviews</a>({ ...params }) -> MarketSDKApi.ReviewList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.reviews.listReviews({
    subject: "subject"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListReviewsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ReviewsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reviews.<a href="/src/api/resources/reviews/client/Client.ts">getReview</a>({ ...params }) -> MarketSDKApi.ReviewObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.reviews.getReview({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetReviewRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ReviewsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Reputation
<details><summary><code>client.reputation.<a href="/src/api/resources/reputation/client/Client.ts">listReputationEvents</a>({ ...params }) -> MarketSDKApi.ReputationEventList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.reputation.listReputationEvents({
    party: "party"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListReputationEventsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ReputationClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reputation.<a href="/src/api/resources/reputation/client/Client.ts">voidReputationEvent</a>({ ...params }) -> MarketSDKApi.ReputationEventObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

For the customer's team. Writes a second event pointing at the first. The voided event stops counting. Nothing is deleted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.reputation.voidReputationEvent({
    id: "id",
    reason: "reason"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.VoidDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ReputationClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Payments
<details><summary><code>client.payments.<a href="/src/api/resources/payments/client/Client.ts">listPayments</a>({ ...params }) -> MarketSDKApi.PaymentList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.payments.listPayments();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListPaymentsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PaymentsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="/src/api/resources/payments/client/Client.ts">getPayment</a>({ ...params }) -> MarketSDKApi.PaymentObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.payments.getPayment({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetPaymentRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PaymentsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="/src/api/resources/payments/client/Client.ts">updatePayment</a>({ ...params }) -> MarketSDKApi.PaymentObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.payments.updatePayment({
    id: "id",
    body: {
        metadata: {
            "key": "value"
        }
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.UpdatePaymentRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PaymentsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="/src/api/resources/payments/client/Client.ts">retryPaymentRelease</a>({ ...params }) -> MarketSDKApi.PaymentObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

For a release that failed, for example because the seller could not yet receive transfers. A release is also tried again by itself when the seller becomes able to receive payouts.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.payments.retryPaymentRelease({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.RetryPaymentReleaseRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PaymentsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="/src/api/resources/payments/client/Client.ts">listRefunds</a>({ ...params }) -> MarketSDKApi.RefundList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.payments.listRefunds();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListRefundsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PaymentsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="/src/api/resources/payments/client/Client.ts">createRefund</a>({ ...params }) -> MarketSDKApi.RefundObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Recorded at once with status `pending`, then made at Stripe. If the seller's share was already released, the transfer is reversed in the same proportion, so your fee is given back in proportion too.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.payments.createRefund();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateRefundDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PaymentsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="/src/api/resources/payments/client/Client.ts">getRefund</a>({ ...params }) -> MarketSDKApi.RefundObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.payments.getRefund({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetRefundRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PaymentsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="/src/api/resources/payments/client/Client.ts">updateRefund</a>({ ...params }) -> MarketSDKApi.RefundObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.payments.updateRefund({
    id: "id",
    body: {
        metadata: {
            "key": "value"
        }
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.UpdateRefundRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PaymentsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Trust
<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">createVerification</a>({ ...params }) -> MarketSDKApi.VerificationObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a Stripe Identity session on your Stripe account and returns its page, once. Only the outcome and the session id are kept; no document image or document data. When seller verification is on, a seller can publish only once verified.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.createVerification({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateVerificationDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">listVerifications</a>({ ...params }) -> MarketSDKApi.VerificationList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.listVerifications();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListVerificationsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">getVerification</a>({ ...params }) -> MarketSDKApi.VerificationObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.getVerification({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetVerificationRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">cancelVerification</a>({ ...params }) -> MarketSDKApi.VerificationObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.cancelVerification({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CancelVerificationRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">listDisputes</a>({ ...params }) -> MarketSDKApi.DisputeList</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Filter by `stage` for a queue.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.listDisputes();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListDisputesRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">getDispute</a>({ ...params }) -> MarketSDKApi.DisputeObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.getDispute({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetDisputeRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">listDisputeEvidence</a>({ ...params }) -> MarketSDKApi.DisputeEvidenceList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.listDisputeEvidence({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListDisputeEvidenceRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">addDisputeEvidence</a>({ ...params }) -> MarketSDKApi.DisputeEvidenceObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Only while the dispute is in its evidence stage.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.addDisputeEvidence({
    id: "id",
    actor: "actor",
    body: "body"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.AddEvidenceDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">closeDisputeEvidence</a>({ ...params }) -> MarketSDKApi.DisputeObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.closeDisputeEvidence({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CloseDisputeEvidenceRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">decideDispute</a>({ ...params }) -> MarketSDKApi.DisputeObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Your team's decision: who it went against, in writing, and with payments on, how much goes back to the buyer. On a claimed order, deciding against the party who disputed upholds the claim and completes the order; deciding against the claimant cancels it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.decideDispute({
    id: "id",
    against: "buyer",
    note: "note"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.DecideDisputeDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="/src/api/resources/trust/client/Client.ts">openDispute</a>({ ...params }) -> MarketSDKApi.DisputeObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

On a claimed order, by the party who did not claim: the order becomes disputed. On a completed order, by either party inside the dispute window: the order stays completed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.trust.openDispute({
    id: "id",
    actor: "buy_034XtPDs7UJ0TXzTsdaHZa",
    reason: "reason"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.OpenDisputeDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `TrustClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Moderation
<details><summary><code>client.moderation.<a href="/src/api/resources/moderation/client/Client.ts">listFlags</a>({ ...params }) -> MarketSDKApi.FlagList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.moderation.listFlags();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListFlagsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ModerationClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="/src/api/resources/moderation/client/Client.ts">createFlag</a>({ ...params }) -> MarketSDKApi.FlagObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

On behalf of the end user who reported it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.moderation.createFlag({
    target: "lst_034XtPDs7UJ0TXzTsdaHZa",
    reporter: "buy_034XtPDs7UJ0TXzTsdaHZa",
    reason: "prohibited_item"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateFlagDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ModerationClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="/src/api/resources/moderation/client/Client.ts">getFlag</a>({ ...params }) -> MarketSDKApi.FlagObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.moderation.getFlag({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetFlagRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ModerationClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="/src/api/resources/moderation/client/Client.ts">getModerationQueue</a>({ ...params }) -> MarketSDKApi.ModerationQueueObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.moderation.getModerationQueue();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetModerationQueueRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ModerationClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="/src/api/resources/moderation/client/Client.ts">listModerationActions</a>({ ...params }) -> MarketSDKApi.ModerationActionList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.moderation.listModerationActions();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListModerationActionsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ModerationClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="/src/api/resources/moderation/client/Client.ts">createModerationAction</a>({ ...params }) -> MarketSDKApi.ModerationActionObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Resolves the target's open flags and logs who acted and why.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.moderation.createModerationAction({
    target: "target",
    action: "dismiss",
    reason: "reason",
    actor: "actor"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateModerationActionDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `ModerationClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Webhooks
<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">listWebhookEndpoints</a>({ ...params }) -> MarketSDKApi.WebhookEndpointList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.listWebhookEndpoints();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListWebhookEndpointsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">createWebhookEndpoint</a>({ ...params }) -> MarketSDKApi.WebhookEndpointObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the signing secret, once. Every delivery carries `MarketSDK-Signature: t=<time>,v1=<HMAC-SHA256 of "<time>.<body>">`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.createWebhookEndpoint({
    url: "https://shop.example/marketsdk/webhooks",
    enabled_events: ["*"]
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.CreateWebhookEndpointDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">getWebhookEndpoint</a>({ ...params }) -> MarketSDKApi.WebhookEndpointObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.getWebhookEndpoint({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetWebhookEndpointRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">deleteWebhookEndpoint</a>({ ...params }) -> MarketSDKApi.DeletedWebhookEndpointObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.deleteWebhookEndpoint({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.DeleteWebhookEndpointRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">updateWebhookEndpoint</a>({ ...params }) -> MarketSDKApi.WebhookEndpointObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.updateWebhookEndpoint({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.UpdateWebhookEndpointDto` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">rotateWebhookSecret</a>({ ...params }) -> MarketSDKApi.WebhookEndpointObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the new secret, once. The old one stops at once.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.rotateWebhookSecret({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.RotateWebhookSecretRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">listWebhookDeliveries</a>({ ...params }) -> MarketSDKApi.WebhookDeliveryList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.listWebhookDeliveries();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListWebhookDeliveriesRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">getWebhookDelivery</a>({ ...params }) -> MarketSDKApi.WebhookDeliveryObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.getWebhookDelivery({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetWebhookDeliveryRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">replayWebhookDelivery</a>({ ...params }) -> MarketSDKApi.WebhookDeliveryObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a new delivery of the same event to the same endpoint.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.replayWebhookDelivery({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ReplayWebhookDeliveryRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">listEvents</a>({ ...params }) -> MarketSDKApi.EventList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.listEvents();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.ListEventsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="/src/api/resources/webhooks/client/Client.ts">getEvent</a>({ ...params }) -> MarketSDKApi.EventObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.webhooks.getEvent({
    id: "id"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `MarketSDKApi.GetEventRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WebhooksClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

