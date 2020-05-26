# Gilded Rose Refactoring Kata

Hi and welcome to team Gilded Rose. As you know, we are a small inn with a prime location in a
prominent city ran by a friendly innkeeper named Allison. We also buy and sell only the finest goods.
Unfortunately, our goods are constantly degrading in quality as they approach their sell by date. We
have a system in place that updates our inventory for us. It was developed by a no-nonsense type named
Leeroy, who has moved on to new adventures. Your task is to add the new feature to our system so that
we can begin selling a new category of items. First an introduction to our system:

- All items have a `sellIn` value which denotes the number of days we have to sell the item
- All items have a `quality` value which denotes how valuable the item is
- At the end of each day our system adjusts both values for every item

Pretty simple, right? Well this is where it gets interesting:

- Once the sell by date has passed, `quality` degrades twice as fast
- The `quality` of an item is **never negative**
- _"Aged Brie"_ actually increases in `quality` the older it gets
- The `quality` of an item is never more than `50`
- _"Sulfuras"_, being a legendary item, never has to be sold or decreases in `quality`
- _"Backstage passes"_, like Aged Brie, increases in `quality` as its `sellIn` value approaches
  - `quality` increases by `2` when there are `10` days or less and by `3` when there are `5` days or less
  - `quality` drops to `0` after the concert

We have recently signed a supplier of conjured items. This requires an update to our system:

- _"Conjured"_ items degrade in `quality` twice as fast as normal items

Feel free to make any changes to the `updateQuality` method and add any new code as long as everything
still works correctly. However, do not alter the Item class or Items property as those belong to the
goblin in the corner who will insta-rage and one-shot you as he doesn't believe in shared code
ownership (you can make the UpdateQuality method and Items property static if you like, we'll cover
for you).

Just for clarification, an item can never have its Quality increase above 50, however _"Sulfuras"_ is a
legendary item and as such its `quality` is `80`, and it never alters.

[![Floobits Status](https://floobits.com/cromeroz-globant/GildedRose-Kata.svg)](https://floobits.com/cromeroz-globant/GildedRose-Kata/redirect)