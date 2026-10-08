# FAQ and troubleshooting

<details>

<summary>A point doesn't show up in game</summary>

Check the icon in the panel: dim means it isn't placed. Then run `/garagecheck`, `/documenticheck` or `/frigocheck` for what the resource sees for your job.

</details>

<details>

<summary>"Item doesn't exist" when printing or billing</summary>

Add the items from [Inventory items](../getting-started/inventory-items.md) and restart ox\_inventory.

</details>

<details>

<summary>The database shows errors on start</summary>

The console names the missing table or column in red. Run `/bkdbcheck` after fixing it. Check that oxmysql starts before the resource.

</details>

<details>

<summary>A flyer or poster shows a blank sheet</summary>

The image link expired (Discord links last about a day) or the host isn't in `Config.Flyers.hosts`.

</details>

<details>

<summary>The DJ booth plays nothing</summary>

xsound must be started. The panel says so when it isn't.

</details>

<details>

<summary>Do I need to restart after changing something?</summary>

No. Jobs, points, recipes and settings apply immediately to everyone.

</details>
