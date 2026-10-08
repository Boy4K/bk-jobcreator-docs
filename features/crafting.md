# Crafting

The hammer icon places the workbenches; **Crafting recipes** (in the list of positions) edits the recipes.

<figure><img src="https://raw.githubusercontent.com/Boy4K/bk-jobcreator-docs/main/assets/crafting.jpg" alt="Recipes and where the ingredients come from"><figcaption><p>Recipes and where the ingredients come from</p></figcaption></figure>

## Recipes

Each recipe has: ingredients, the item it gives and how many, a **craft type** (sound + animation + duration from `Config.CraftTypes`), an object in hand, the direction to face, and the **XP** it gives. **Try in game** previews the animation.

## Ingredients from a company storage

Under the recipes, **Where the ingredients come from**:

* **From the crafter's inventory** – as usual.
* **From the storage: …** – any **shared** storage of the job. What's in the storage is used first, then the crafter's inventory.
* **From the job fridge** – the crafter's own fridge (fridges are personal in ox\_inventory), if the job has one placed.

With a storage or the fridge you also choose **where the product goes**: the crafter's inventory or the same place. If it's full, the product goes to the crafter.

{% hint style="info" %}
The storage grade is respected: someone who can't open that storage crafts only from their own inventory.
{% endhint %}

## Checked by the server

The server finds the recipe in the job file, checks the ingredients, that the player is at one of the job's workbenches (8 m), and gives everything back if something fails halfway.
