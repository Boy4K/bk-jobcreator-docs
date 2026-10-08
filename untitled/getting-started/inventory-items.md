# Inventory items

Add these to `ox_inventory/data/items.lua`, then restart ox\_inventory.

```lua
['bill'] = {
    label = 'Invoice',
    weight = 0,
    stack = false,      -- each invoice is its own piece of paper
    close = true,
    description = 'An unpaid invoice',
    client = { export = 'bk_jobcreator.useBillItem' }
},

['documento'] = {
    label = 'Document',
    weight = 10,
    stack = false,
    close = true,
    consume = 0,
    client = { export = 'bk_jobcreator.useDocument' }
},

['volantino'] = {
    label = 'Flyer',
    weight = 1,
    stack = true,
    close = true,
    consume = 0,
    client = { export = 'bk_jobcreator.useFlyer' }
},

['giornale'] = {
    label = 'Newspaper',
    weight = 1,
    stack = true,
    close = true,
    consume = 0,
    client = { export = 'bk_jobcreator.useFlyer' }
},
```

{% hint style="warning" %}
Keep `stack = false` on `bill` and `documento`: each one carries its own number in its metadata.
{% endhint %}

The item names can be changed in `shared/config.lua` (`Config.Billing.item`, `Config.Documents.item`, `Config.Flyers.items`). Keep the two in step.

## Food that spoils (optional)

For the [fridge](../features/fridge.md): give the food a `degrade` (minutes) in `items.lua` and list it in `Config.Fridge.PerishableItems`. Use `stack = false` on food, since every piece carries its own countdown.

```lua
PerishableItems = {
    burger = { spoiledItem = 'rotten_food' },
    apple  = {},   -- just disappears at 0%
}
```
