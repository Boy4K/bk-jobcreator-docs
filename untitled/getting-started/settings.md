# Settings panel

Open the staff panel and click the **gear** next to the title. Settings apply to the whole server **immediately**, for everyone, and are saved in `settings.json`.

| Setting                 | Options                                                                                                                     |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| **Language**            | English or Italiano: panel, menus, notifications, cloakroom, crafting, documents. ox\_target labels rebuild on their own.   |
| **Notifications**       | ESX (default) or ox\_lib, with position and duration. **Test the notification** shows it before saving.                     |
| **Currency**            | symbol, before or after the amount, 1,250 or 1.250 (live example)                                                           |
| **Tax cap**             | the highest value `/settax` can set (0–100%)                                                                                |
| **Positions per point** | how many positions each point can have (1–50, default 10)                                                                   |
| **Posters around town** | on/off, hours before they expire, how many per player and in the whole town, who can tear them down, **Remove all posters** |

{% hint style="info" %}
`shared/config.lua` is the starting point. Whatever you save from the panel wins over it. **Reset to config.lua** goes back to the file values.
{% endhint %}
