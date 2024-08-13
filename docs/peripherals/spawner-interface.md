# Spawner Interface
---

Allows for manipulating spawners

| Functions | Description |
| - | - |
| [getCurrentlySpawningMob()](#getcurrentlyspawningmob) | Gets the current spawning mob in the spawner |
| [captureSpawner([ inventory ], [ slot ])](#capturespawner-inventory-slot) | Makes the spawner drop itself |
| [changeSpawner(inventory, slot, [ force ])](#changespawnerinventory-slot-force) | Makes the spawner swap what mob it spawns |

### getCurrentlySpawningMob()

**Description**
---
Gets the current spawning mob in the spawner

**Returns**

1. boolean | string - The state of the operation or the id of the spawning mob
2. string - Error message, If there is a failure on the operation

### captureSpawner([ inventory ], [ slot ])
---
**Description**

Makes the spawner drop itself

if the parameters are passed store the current mob on a spawner card.

**Parameters**

1. inventory: string - a inventory that has a spawner card
2. slot: number - the slot where the spawner card is located

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

### changeSpawner(inventory, slot, [ force ])
---
**Description**

Makes the spawner swap what mob it spawns


**Parameters**

1. inventory: string - a inventory that has a spawner card
2. slot: number - the slot where the spawner card is located
3. ?force: boolean - if set, the mob that was in the spawner is discarted

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

