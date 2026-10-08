# Invoices

Jobs with invoices on can bill players: target a player, or `/bill [id]`.

* **The POS:** keypad, quick amounts, reason. The **state tax** is shown before sending: how much goes to the state and how much the company keeps.
* **The customer** gets a `bill` item with the receipt and a barcode, and pays by bank transfer.
* **The tax:** `/settax <percent>`, used by the government boss or staff, up to the tax cap in [Settings](../getting-started/settings.md).
* **Turning it on:** in the job editor, or `/billjob <job> on|off`.
