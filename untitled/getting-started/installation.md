# Installation

{% stepper %}
{% step %}
### Copy the resource

Put the `bk_jobcreator` folder in your `resources` folder.
{% endstep %}

{% step %}
### Add the inventory items

Add the four items from [Inventory items](inventory-items.md) to `ox_inventory/data/items.lua`.
{% endstep %}

{% step %}
### Start order

In `server.cfg`, start it **after** its dependencies:

```
ensure es_extended
ensure ox_lib
ensure oxmysql
ensure ox_target
ensure ox_inventory
ensure bk_jobcreator
```
{% endstep %}

{% step %}
### Start the server

The resource creates and checks its own database tables on start. If something is missing, the console says which table or column in red.

Run `/bkdbcheck` at any time to check the database again.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
`install.sql` is still included as a safety net. You don't need to import it: the resource does the same on start.
{% endhint %}

## Who can open the panel

Staff groups are listed in `Config.AdminGroups` in `shared/config.lua` (by default `owner`, `admin`, `superadmin`). Open the panel with `/jobcreator`.

## Where things are saved

| File                   | What                                                                     |
| ---------------------- | ------------------------------------------------------------------------ |
| `jobs/<job>.json`      | everything about a job: points, storages, garage, crafting, documents... |
| `settings.json`        | the settings changed from the panel                                      |
| `workzones/zones.json` | the work zones                                                           |
| `posters.json`         | the posters stuck on walls                                               |

All of them are written by the resource. You never need to edit them by hand.
