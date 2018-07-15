
#NOTE
This is not a idea production application.
This is to be used for educational purpose only

## test-your-restaurant
Is your restaurant good enough ?

Restaurant with pages 
* Menu & Order
* Inventory
* Profile

### Menu 
    Show all items from inventory
    If the availability of item is sold_out disable add button
    No quantity is required in order page

Actions
| ACTION_TYPE | Description |
| ------ | ------ |
| ADD_TO_ORDER | Add item to user's order |


### Order 
    Show all items from inventory
    If the availability of item is sold_out disable add button
    No quantity is required in order page
    Calculate Total every time an item is added to order

Actions
| ACTION_TYPE | Description |
| ------ | ------ |
| REMOVE_FROM_ORDER | Remove item from user's order |
| CALC_TOTAL | Calculate total on adding dish to order |


### Inventory
Inventory page should list items available.

Actions
| Description | ACTION_TYPE |
| ------ | ------ |
| Add dish to inventory | ADD_DISH |
| Remove dish from inventory  | REMOVE_DISH|
| Change Properties of dih in inventory (ie) Price, Name, Description, image etc | UPDATE_DISH |
| Change Avialability of dish  | UPDATE_AVAILABILITY|
| Bulk Upload to inventory  | UPLOAD_DISH|

Use the available json for bulk upload


### Store Structure
```json
{
    dishes: {
    },
    order:[
        {
            "name": "Creamy Cheesy Pasta",
            "image": "/images/pasta.jpg",
            "desc": "Creamy Cheesy Pasta",
            "price": 2250,
            "status": "available"
        },
    ]
}
```
