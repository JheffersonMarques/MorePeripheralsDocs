# Magnetic Card Manipulator
---

Allows the reading and writing of [Magnetic Cards](../items/magnetic-card.md)

| Functions | Description |
| - | - |
| [readCard()](#readcard) | Read a card data |
| [writeCard(data)](#writecarddata) | Writes a card data |
| [hasCard()](#hascard) | Check the presence of a card |
| [ejectCard()](#ejectcard) | Drops the current card |
| [setLabel(label)](#setlabellabel) | Sets a card label |
| [getLabel()](#getlabel) | Gets the card's label |
| [setSecure(value)](#setsecurevalue) | Sets if the card should hide the its data tooltip |

### readCard()
---

**Description**

Read a card data

**Returns**

1. boolean | string - The state of the operation or data string
2. string - Error message, If there is a failure on the operation 

### writeCard(data)
---

**Description**

Writes a card data

**Parameters**

1. data: string - the value to store

**Returns**

1. boolean - The state of the operation 
2. string - Error message, If there is a failure on the operation 

### hasCard()
---

**Description**

Check the presence of a card

**Returns**

1. boolean - if there is a card present

### ejectCard()

**Description**

Drops the current card

**Returns**

1. boolean - if could drop the card

### setLabel(label)

**Description**

Sets a card label 

**Parameters**

1. label: string - the label to set

**Returns**

1. boolean - if rename the card

### getLabel()

**Description**

Gets the card's label

**Returns**

1. boolean | string - The state of the operation or the label
2. string - Error message, If there is a failure on the operation 

### setSecure(value)

**Description**

Sets if the card should hide the its data tooltip

**Parameters**

1. value: boolean - the sensibility flag

**Returns**

1. boolean | string - The state of the operation or the label
2. string - Error message, If there is a failure on the operation 