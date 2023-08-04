# Grindstone
---

Allows interactions with the grindstone

| Functions | Description |
| - | - |
| [combine(from, fromSlot, resource, resourceSlot)](#combinefrom-fromslot-resource-resourceslot) | Combine items following the rules of the grindstone |
| [disenchant(from, slot, [ collector ])](#disenchantfrom-slot-collector) | Desenchants an item |


### combine(from, fromSlot, resource, resourceSlot)

---

**Description**

Combine items following the rules of the grindstone

**Paramenters**

1. from : string - The inventory from where the base item is located
2. fromSlot : number - The slot where the base item is present
3. resources : string - The inventory from where the item that will be combined is located
4. resourcesSlot : number - The slot where the combined item is present

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

### disenchant(from, slot, [ collector ])

---
**Description**

Desenchants an item

**Paramenters**

1. from : string - The inventory from where the item is located
2. slot : number - The slot where the item is present
3. ?collector : string - An experience collector to recieve the XP from the disenchanting process

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation
