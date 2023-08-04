# Loom
---
Allows the for banner manipulation

| Functions | Description |
| - | - |
| [paintBanner(input, bannerSlot, dyeSlot, pattern)](#paintbannerinput-bannerslot-dyeslot-pattern) |  Paints a pattern on a banner (consumes dyes equivalent to the quantity of banners) |
| [clearBanner(input, slot)](#clearbannerinput-slot) | Clear all patterns on a banner |

### paintBanner(input, bannerSlot, dyeSlot, pattern)

---

**Description**

Paints a pattern on a banner (consumes dyes equivalent to the quantity of banners)

**Parameters**

1. input: string - Inventory where the items are located
2. bannerSlot: number - Slot referring to the banner to be painted
3. dyeSlot: number - Slot referring to the dye used to paint
4. pattern: number - An integer that defines a banner pattern

**Returns**

1. boolean - The state of the operation or if there are bees inside of the hive
2. string - Error message, If there is a failure on the operation 


### clearBanner(input, slot)

---

**Description**

Clear all patterns on a banner

**Parameters**

1. input: string - Inventory where the items are located
2. slot: number - Slot referring to the banner to be cleared

**Returns**

1. boolean - The state of the operation or if there are bees inside of the hive
2. string - Error message, If there is a failure on the operation 
