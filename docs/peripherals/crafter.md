# Crafter
---
Allows Autocrafting without the need to have a crafting turtle or a turtle at all

| Functions | Description |
| - | - |
| [craft(from, to, recipe)](#craftfrom-to-recipe) | Crafting an item if the recipes match |


### craft(from, to, recipe)

---
**Description**

Crafting an item if the recipes match

**Parameters**

1. from: string - Inventory to get crafting items
2. to: string - Inventory to send the crafted items
3. recipe: table - A list of slots defining the structure of the recipe

> 💡 IMPORTANT
> 
> The recipe table is an array of size 9, where the value in the array defines the slot that the crafter will try to use
> 
> If there is a 0, no slot is picked


**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation 

**Usage**

```lua title="Chest Crafting Example"

local crafter = peripheral.wrap("crafter");

-- Inventory to get items from
local inputInv = peripheral.wrap("minecraft:chest_0")   

-- Inventory to store items crafted
local outputInv = peripheral.wrap("minecraft:chest_1")  

-- Assuming there are planks in the first slot of the input chest
local state, err = crafter.craft(
    peripheral.getName(inputInv),
    peripheral.getName(outputInv),
    {
      1,1,1,
      1,0,1,
      1,1,1
    }
)

if(err) -- If there was an error, display the error message
    error(err)

print(state); -- Display if could craft the item
```