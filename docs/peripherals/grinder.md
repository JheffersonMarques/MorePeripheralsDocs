# Grinder
---

A mob grinder that can utilize any sword, and applies its effects like Fire Aspect or Sharpness
Hitting on a 3x3 Area Around it.


| Functions | Description |
| - | - |
| [attack()](#attack) |Attack any living mob around it (apply sword enchantments) |
| [hasSword()](#hasSword) | Returns a boolean if the grinder has a sword in it |
| [pullSword(from, slot)](#pullswordfrom-slot) | Pulls a sword from the target inventory |
| [pushSword(to)](#pushswordto) | Pushes a sword to the target inventory |


### attack()

---
**Description**

Attack any living mob around it (apply sword enchantments)

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

### hasSword()

---
**Description**

Returns a boolean if the grinder has a sword in it

**Returns**

1. boolean - If there is any sword in the grinder

### pullSword(from, slot)
---
**Description**

Pulls a sword from the target inventory

**Parameters**

1. from: string - Inventory from where to get the sword
2. slot: number - The slot for the sword


**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

### pushSword(to)

---

**Description**

Pushes a sword to the target inventory

**Parameters**

1. to: string - Inventory from where to send the sword

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation