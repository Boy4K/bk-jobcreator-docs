# Jobs and points

Each row in the panel is a job; each icon is one of its points.

<figure><img src="https://raw.githubusercontent.com/Boy4K/bk-jobcreator-docs/main/bk-jobcreator-docs/assets/staff-panel.jpg" alt="Three jobs and their points"><figcaption><p>Three jobs and their points</p></figcaption></figure>

* **Icon colour:** highlighted when the point is ready, red when something is missing, dim when it isn't set.
* **The number** on an icon tells how many positions that point has.
* **Under each icon:** a pin that teleports to the first position, and a bin that opens the list or the manager so you choose what to remove.

## Creating and editing a job

**Create job** asks for the job ID, the name and the highest grade, then the grades one by one (internal name, shown name, salary). **Edit** changes all of it later, plus:

* **Whitelist only** – untick for a job anyone can take.
* **Invoices** – lets the job bill players.
* **Duty** – on/off duty from the [F6 menu](duty-menu.md).
* **Law enforcement** – radio alerts to colleagues when someone goes on or off duty.

<figure><img src="https://raw.githubusercontent.com/Boy4K/bk-jobcreator-docs/main/bk-jobcreator-docs/assets/job-edit.jpg" alt="Editing a job"><figcaption><p>Editing a job</p></figcaption></figure>

## Deleting a job

**Delete** asks for a second click. It removes the job and its grades, the company account, its work zones, unpaid invoices and duty backups, and sets every employee to unemployed. Jobs the server needs (`unemployed`, the off-duty job) can't be deleted.
