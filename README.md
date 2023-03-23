# InventoryHelper

## The Basics
### Example of each function (adding a item, removing a item, rendering hotbar)
``` Lua
-- Getting the module from the SeverScriptService

local inventoryHelper = require(game:GetService("ServerScriptService"):WaitForChild("InventoryHelper"))

-- Initilize the module
-- p = player object (normally would get this from PlayerAdded Function)
local inventory = inventoryHelper.new(p) 

--Add a item (ItemName, Amount)
-- Example of adding 3 oak_wood
inventory:addItem('oak_wood',3)

--Remove a item (ItemName, Amount)
-- Example of removing 2 dark_oak_wood
inventory:removeItem('dark_oak_wood', 2)

-- Render the items in the hotbar
inventory:renderHB()
```
<hr>

# Methods
## Inventory:`additem`(itemName:String, amount:number)
``` Lua
inventory:addItem(Item Name, Amount)
```
> Item Name = String
> Amount = number / integer
> addItem takes two parameters the name of the item you want to add and quantity
> 
<hr>

## Inventory:`removeItem`(temName:String, amount:number)
``` Lua
inventory:renderHB()
```
> Item Name = String
> Amount = number / integer
> removeItem takes two parameters the name of the item you want to remove and quantity
<hr>
## Inventory.`new`(player)
```Lua
local inventory = inventory.new(player)
```
> takes a player object parameter
> this sets up the inventory var as a inventoryHelper object
> Reason:
> instead of having to do inventory:addItem(player, item, amount)
> we don't have to pass the player object because we save it when we use the .new method
 
