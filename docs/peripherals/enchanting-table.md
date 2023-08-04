# Ender Chest Interface
---

Allows for automated enchanting and getting information about enchantments

| Functions | Description |
| - | - |
| [getEnchantsFor(from, slot)](#getenchantsforfrom-slot) | Gets all possible enchantments for the item |
| [enchant(from, slot, resources)](#enchantfrom-slot-resources) | Enchants an item with a random supported enchantment, if there is enough resources to do so |


### getEnchantsFor(from, slot)

---
**Description**

Gets all possible enchantments for the item

**Parameters**

1. from: string - Inventory from where to get the item
2. slot: number - The slot for the item


**Returns**

1. boolean - The state of the operation
2. string | table - Error message, If there is a failure on the operation or a table with a list for all supported enchantments

### enchant(from, slot, resources)

---
**Description**

Enchants an item with a random supported enchantment, if there is enough resources to do so

**Parameters**

1. from: string - Inventory from where to get the item to enchant
2. slot: number - The slot for the item to enchant
3. resources: string - Inventory with the needed resources to do the enchantment


> 💡 IMPORTANT
>
> The enchantment process consumes 8 Bottles o' Enchanting and 1 lapis lazuli per enchant

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation 
