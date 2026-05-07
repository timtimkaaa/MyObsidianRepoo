### Description

This is an app that helps users plan their shopping and navigate the store quickly and efficiently.
It allows to CRUD lists of products for a store on Lists screen, see prices with promotions, set quantity (or weight), sort the products. It let's users see promotions on Promotions screen. Users can search, sort and filter products on Search screen, see details about these products on Details screen and add them to different lists. The app has a Locate function to show the product's location on Locate screen with a map and a pin for the product (it doesn't show user's location). Lastly the app has a Navigation screen, where the user can see the optimal route for a list and check off an item they just got (thus letting the app know where they are in the store right now). 
This app uses Supabase for backend (with their authentication system), JS for app logic and React Native for UI.

### Class diagram

Store 
- id
- name

StoreMapService
+ getSections()  
+ buildMap(sections, grid)

StoreMap
- sections: Section[]
- grid: number[][]

Section
- id
- storeId
- name
- x
- y

ProductService
+ getProductPreviews()  
+ getProductPreviewsByStore(store)  
+ getProductById(id)

Product (combined Product and StoreProduct data)
- id  
- name  
- category  
- description  
- thumbnail  
- picture  
- price  
- discount  
- section

RoutePlanner
+ calculateRoute(products)  
+ findPath(start, end)

ShoppingListService
+ createList()  
+ removeList()  
+ addItem(list: ShoppingList)  
+ removeItem(list: ShoppingList)  
+ sort(list: ShoppingList)  
+ markCollected(productId)  
+ markFinished()

ShoppingList
- id  
- userId  
- items: ShoppingListItem[]  
- updatedAt  
- isFinished

ShoppingListItem
- shoppingListId
- shoppingListItemId
- product  
- quantity  
- isCollected

SyncService
+ syncShoppingLists()  
+ pushLocalChanges()  
+ fetchRemoteLists()  
+ resolveConflicts()

PromotionService
+ getPromotions()  
+ getPromotionsByStore()  
+ getPromotionById(id)

Promotion
- id  
- product  
- storeId
- picture  
- description  
- discountValue  
- validUntil

AuthService
+ login(email, password)  
+ logout()  
+ getCurrentUser()  
+ isAuthenticated()

StoreMapService (association (+ buildMap(sections, grid))) StoreMap (aggregation (- sections)) Section (association (- storeId)) Store
ProductService (association) Product (association (- section)) Section
ProductService (association (+ getProductsByStore)) Store
RoutePlanner (association (+ calculateRoute(products))) Product
RoutePlanner (association (+ calculateRoute(products))) StoreMap
ShoppingListService (association (+ markCollected(productId))) Product
ShoppingListService (association (+ addItem(), removeItem(), sort())) ShoppingList (composition (- items)) ShoppingListItem (association (- product)) Product
SyncService (association) ShoppingList
AuthService (association) ShoppingList
PromotionService (association (+ get promotionById(id))) Promotion (association ( - storeId)) Store

### ER diagram

Store
- store_id
- name
- address

Section
- section_id
- store_id
- name
- x
- y

StoreProduct
- product_id
- section_id
- store_id
- price
//UNIQUE (store_id, product_id)

Promotion
- promotion_id
- product_id
- store_id
- picture
- description
- discount_value
- valid_until

Product
- product_id
- name
- category
- description
- thumbnail
- picture

ShoppingListItem
- shopping_list_item_id
- shopping_list_id
- product_id
- quantity

ShoppingList
- shopping_list_id
- name
- user_id
- created_at
- updated_at
- is_finished

User 
- user_id
- email
- first_name
- last_name
- password_hash

Store 1:N Section
Store 1:N StoreProduct
Store 1:N Promotion
Section 1:N StoreProduct
User 1:N ShoppingList
ShoppingList 1:N ShoppingListItem
Product 1:N ShoppingListItem
Product 1:N StoreProduct
Product 1:N Promotion