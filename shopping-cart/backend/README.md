
# Application design

## Commands
 - Add item to cart
        AddCartItemCommand (item, datetime)
 - Change item count (increment/decremnet)
        ChangeCartItemCommand (item, number, datetime)
 - Remove item from cart
        RemoveCartItemCommand(item, datetime)        
 - Clear cart
        ClearCartCommand (cart, datetime)
 - Checkout cart
        CheckoutCartCommand (cart, datetime, note)
        
## Queries

## Events
- Item added to cart (one item at a time)
        AddCartItemEvent
- Item(s) removed from (list of items)
        RemovedCartItemEvent
- Cart checkedout
        CheckoutCartEvent
            

## Entities
  - Item
  - Cart
        event-sourced entity
  - Purchase
      
