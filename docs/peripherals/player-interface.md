# Player interface
---

Allows for manipulating the contents of a player inventory and do some action as that player if there is a bound [Player Card](../items/player-card.md)

| Functions | Description |
| - | - |
| [consume(slot)](#consumeslot) | Makes the player eat an edible item in its inventory |
| [lookAt(x, y, z)](#lookatx-y-z) | Makes the player look at a coordinate |
| [displayMessage(msg, [ tooltip ])](#displaymessagemsg-tooltip) | Shows a message to the player |

The inventory functions follows the rules of the [Inventory API](https://tweaked.cc/generic_peripheral/inventory.html), though the player interface isn't itself considered a inventory

### consume(slot)

---
**Description**

Makes the player eat an edible item in its inventory

**Parameters**

1. slot: number - The slot for the edible item item


**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation


### lookAt(x, y, z)

---
**Description**

Makes the player look at a coordinate

**Parameters**

1. x: number - the target's x position,
2. y: number - the target's y position,
3. z: number - the target's z position 


**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation

### displayMessage(msg, [ tooltip ])

---
**Description**

Shows a message to the player

**Parameters**

1. msg: string - a message to be sent
2. ?tooltip: boolean - if the message should be display as a tooltip, instead of a chat message


**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation
