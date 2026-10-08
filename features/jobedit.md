# Boss editor (/jobedit)

The boss of a job types `/jobedit` and moves the points of their job, without staff.

* A point with **one** position moves directly.
* A point with **several** positions opens its list: Position 1, Position 2… and moves the chosen one.
* **Storages** and **DJ consoles** have their own lists.
* Move several points, then **Save and close**, or **Leave without saving**. Closing with ESC keeps the moves until you reopen and save.

Creating or removing points stays with staff.

## What the boss can move

`Config.SelfEdit.allowedZones` in `shared/config.lua`. By default: cloakroom, boss menu, fridge, selling, printer, storages, DJ console and speaker. **Not** crafting and garage: set `crafting = true` to allow workbenches too.
