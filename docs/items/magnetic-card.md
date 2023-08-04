# Magnetic Card
---

A Magnetic Card can store some small amount of data, on right clicking on a [Magnetic Card Manipulator](../peripherals/magnetic-card-manipulator.md) 
sends an `card_read` event that contains the data stored on the card, also placing or removing the card from the magnetic card manipulator sends the `card_insert` and `card_remove` events respectvely

> The cards are dyeable on the latest updates