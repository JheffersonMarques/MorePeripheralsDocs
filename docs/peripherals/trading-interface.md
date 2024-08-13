# Trading Interface
---

Allows for automatic trading and manipulation of some villager properties

| Functions | Description |
| - | - |
| [getProfession()](#getprofession) | Gets the current villager profession  |
| [getTrades()](#gettrades) | Gets all available trades on for a villager |
| [trade(from, to, trade)](#tradefrom-to-trade) | Makes a trade with a villager |
| [restock()](#restock) | Forces a villager to restock its trades |
| [cycleTrades()](#cycletrades) | Forces a villager to reset its trades |

### getProfession()
---
**Description**

Gets the current villager profession 

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation or the profession name

### getTrades()
---
**Description**

Gets all available trades on for a villager

**Returns**

1. boolean - The state of the operation
2. string | table - Error message, If there is a failure on the operation or a table representing the trades

### trade(from, to, trade)
---
**Description**

Makes a trade with a villager

**Parameters**

1. from: string - a inventory from where to get the trade resources
2. to: string - a inventory to place the trade result
3. trade: number - the index of the trade

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

### restock()
---
**Description**

Forces a villager to restock its trades

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

### cycleTrades()
---
**Description**

Forces a villager to reset its trades

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

