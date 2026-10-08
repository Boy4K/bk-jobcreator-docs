# Invoices

Jobs with invoices on can bill players: target a player, or `/bill [id]`.

<div style="display:flex;gap:12px"><img src="https://raw.githubusercontent.com/Boy4K/bk-jobcreator-docs/main/bk-jobcreator-docs/assets/invoice-pos.jpg" alt="The POS" width="45%"><img src="https://raw.githubusercontent.com/Boy4K/bk-jobcreator-docs/main/bk-jobcreator-docs/assets/invoice-receipt.jpg" alt="The receipt" width="45%"></div>

* **The POS:** keypad, quick amounts, reason. The **state tax** is shown before sending: how much goes to the state and how much the company keeps.
* **The customer** gets a `bill` item with the receipt and a barcode, and pays by bank transfer.
* **The tax:** `/settax <percent>`, used by the government boss or staff, up to the tax cap in [Settings](../getting-started/settings.md).
* **Turning it on:** in the job editor, or `/billjob <job> on|off`.
