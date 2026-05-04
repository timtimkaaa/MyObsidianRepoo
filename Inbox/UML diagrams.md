### Description
This is an app that helps users plan their shopping and navigate the store quickly and efficiently.
It allows to CRUD lists of products for a store on Lists screen, see prices with promotions, set quantity (or weight), sort the products. It let's users see promotions on Promotions screen. Users can search, sort and filter products on Search screen, see details about these products on Details screen and add them to different lists. The app has a Locate function to show the product's location on Locate screen with a map and a pin for the product (it doesn't show user's location). Lastly the app has a Navigation screen, where the user can see the optimal route for a list and check off an item they just got (thus letting the app know where they are in the store right now). 

### Class diagrams

StoreMapService
+ getSections()  
+ buildMap(sections, grid)

StoreMap
- sections: Section[]
- grid: number[][]

Section
- id
- store_id
- name
- x
- y

ProductService
+ getProductPreviews()  
+ getProductPreviewsByStore(store)  
+ getProductById(id)

Product
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
+ addItem(list)  
+ removeItem(list: ShoppingList)  
+ sort(list: shoppingList)  
+ markCollected(productId)  
+ markFinishied()

ShoppingList
- id  
- userId  
- items: ShoppingListItem[]  
- updatedAt  
- isFinished

ShoppingListItem
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
- store  
- picture  
- description  
- discountValue  
- validUntil

AuthService
+ login(email, password)  
+ logout()  
+ getCurrentUser()  
+ isAuthenticated()

