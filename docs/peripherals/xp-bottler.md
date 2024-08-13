# XP Bottler
---

Allows players to store xp from a [XP Collector](xp-collector.md) into bottles

| Functions | Description |
| - | - |
| [bottleXP(from, to, xp_collector)](#bottlexpfrom-to-xp_collector) | Store xp in bottles |

### bottleXP(from, to, xp_collector)
---
**Description**

Store xp in bottles

**Parameters**

1. from: string - a inventory from where to get the bottles
2. to: string - a inventory to place the bottled xp
3. xp_collector: string - the xp collector from where to get the XP

**Returns**

1. boolean - The state of the operation
2. string - Error message, If there is a failure on the operation
