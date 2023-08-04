# Beehive Interface
---
Permits retriving information about beehives, and also colleting either the honey comb, or honey bottles using any computer or turtle

The Beehive Interface needs an Beehive or Nest in any of the sides of it to work.

| Functions | Description |
| - | - |
| [hasBees()](#hasbees) | Check if bees are present on the hive |
| [getBeeCount()](#getbeecount) | Checks how many bees are in the hive |
| [gotFireNear()](#gotfirenear) | Checks if there is fire near the hive |
| [getBees()](#getbees) | Gets the state of the bees in the hive |
| [getHoneyLevel()](#gethoneylevel) | Checks the state of the honey inside the hive |
| [collectHoney(resources, output, bottled)](#collecthoneyresources-output-bottled) | Collects the honey |

### hasBees()

---

**Description**

Check if bees are present on the hive

**Returns**

1. boolean - The state of the operation or if there are bees inside of the hive
2. string - Error message, If there is a failure on the operation 

### getBeeCount()

---

**Description**

Checks how many bees are in the hive

**Returns**

1. boolean | number - The state of the operation or the number of bees present
2. string - Error message, If there is a failure on the operation 

### gotFireNear()

---

**Description**

Checks if there is fire near the hive

**Returns**

1. boolean - The state of the operation or the if there is fire close to the hive
2. string - Error message, If there is a failure on the operation 

### getBees()

---

**Description**

Gets the state of the bees in the hive

**Returns**

1. boolean | table - The state of the operation or the state of the bees on the hive
2. string - Error message, If there is a failure on the operation 

### getHoneyLevel()

---

**Description**

Checks the state of the honey inside the hive

**Returns**

1. boolean | number - The state of the operation or a number representing the honey level (1..5)
2. string - Error message, If there is a failure on the operation

### collectHoney(resources, output, bottled)

---

**Description**

Collects the honey as honey bottles or honeycombs

**Parameters**

1. resources: string - The input from where to source bottles or shears
2. output: string - The place where to put the collected resources
3. bottled: boolean - If true the will collect honey bottles, if false will collect honeycombs

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

**Usage**

```lua title="Honey Collection Example"
local beehive = peripheral.find("beehive_interface");
local state, err = beehive.collectHoney("left","top", false);

if(err) -- If there was an error, display the error message
    error(err)

print(state); -- Display if could collect from the hive
```