# Anvil
---

Allows computers to use anvils as peripherals

| Functions | Description |
| - | - |
| [combine(from,fromSlot, resources, resourcesSlot, xpSource)](#combinefrom-fromslot-resources-resourcesslot-xpsource) | Combines items from inside of inventories accesible to the computers via the [Inventory API](https://tweaked.cc/generic_peripheral/inventory.html), using 8 Bottles o' Enchanting per item. |
| [rename(from,slot,name)](#renamefrom-slot-name) | Renames an item with the name given |


### combine(from, fromSlot, resources, resourcesSlot, xpSource)

---

**Description**

Combines items from inside of inventories accesible to the computers via the [Inventory API](https://tweaked.cc/generic_peripheral/inventory.html), using 8 Bottles o' Enchanting per item.


**Parameters**

1. from : string - The inventory from where the base item is located
2. fromSlot : number - The slot where the base item is present
3. resources : string - The inventory from where the item that will be combined is located
4. resourcesSlot : number - The slot where the combined item is present
5. xpSource : string - An inventory from which the xp bottles will be used to combine the items

**Returns**

1. boolean - The state of the operation
2. string - error message, If there is a failure on the operation


**Usage**

```lua title="Item Combine Example"
local anvil = peripheral.find("anvil_interface");
local state, err = anvil.combine("left",1,"right",1,"top");

if(err) -- If there was an error, display the error message
    error(err);

print(state); -- Display if could combine items
```

### rename(from, slot, name)

---

**Description**

Renames an item with the name given


**Parameters**

1. from : string - The inventory from where the base item is located
2. slot : number - The slot where the base item is present
3. name : string - The name to be set for the item


**Returns**

1. boolean - The state of the operation
2. string - error message, If there is a failure on the operation

**Usage**

```lua title="Item Rename Example"
local anvil = peripheral.find("anvil_interface");
local state, err = anvil.rename("left",1,"Very Nice Looting Sword");

if(err) -- If there was an error, display the error message
    error(err);

print(state); -- Display if could rename the item
```