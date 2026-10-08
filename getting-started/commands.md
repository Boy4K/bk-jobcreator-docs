# Commands and permissions

| Command | Who | What it does |
| --- | --- | --- |
| `/jobcreator` | staff | opens the staff panel |
| `/jobedit` | job boss | moves the points of their own job ([Boss editor](../features/jobedit.md)) |
| `F6` / `/jobmenu` | everyone | the job menu: go on and off duty |
| `/bill [id]` | jobs with invoices on | opens the POS for that player |
| `/billjob <job> on\|off` | staff | turns invoices on or off for a job |
| `/settax <percent>` | government boss, staff | sets the state tax on invoices (up to the tax cap) |
| `/workzone` | staff | starts drawing a work zone |
| `/documento <number>` | staff | opens any printed document (for in-game disputes) |
| `/resetlocker <id> [job]` | staff | resets a player's locker code |
| `/companies` | staff | balances of every company |
| `/bkdbcheck` | console, staff | checks the database tables and columns |

**Staff** means the groups in `Config.AdminGroups`.

## Diagnostic commands

`/billcheck`, `/garagecheck`, `/documenticheck`, `/frigocheck` print what the resource sees for your current job. Useful when a point doesn't show up.
