
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

| ACTION_TYPE | Description
| ------ | ------
| ADD_TO_ORDER | Add item to user's order


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

| ACTION_TYPE | Description |
| ------ | ------ |
| ADD_DISH | Add dish to inventory |
| REMOVE_DISH | Remove dish from inventory |
| UPDATE_DISH | Change Properties of dih in inventory (ie) Price, Name, Description, image etc |
| UPDATE_AVAILABILITY | Change Avialability of dish |
| UPLOAD_DISH | Bulk Upload to inventory|

Use the available json for bulk upload


### Store Structure
```js
{
    dishes: {
    },
    order:[
        {
            "id":"ITEM001"
            "name": "Creamy Cheesy Pasta",
            "price": 2250,
            "status": "available"
        },
    ]
}
```
