# Translations

All visible text lives in two files with the same keys:

| File | Language |
| --- | --- |
| `shared/locales.lua` | Italiano (base) |
| `shared/locales_en.lua` | English |

To change a text, edit the value on the right, never the key on the left. Keep `%s`, `%d`, `%%`, `\n` and `<b>` where they are. A key missing from the English file shows the Italian text instead of breaking.

The language is chosen in [Settings](../getting-started/settings.md).
