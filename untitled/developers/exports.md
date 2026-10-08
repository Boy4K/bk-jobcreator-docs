# Exports

All server-side.

```lua
-- company money
exports.bk_jobcreator:GetSocietyMoney(job)            -- number
exports.bk_jobcreator:AddMoneyToSociety(job, amount)   -- true/false
exports.bk_jobcreator:RemoveMoneyFromSociety(job, amount)
exports.bk_jobcreator:GetSocietyTax(job)

-- jobs
exports.bk_jobcreator:ReloadJobs()
exports.bk_jobcreator:GetBossJobs()

-- work zones
exports.bk_jobcreator:GetWorkZones()
exports.bk_jobcreator:GetWorkLitter()

-- lockers
exports.bk_jobcreator:GetLockerStash(identifier, jobName)
```

{% hint style="warning" %}
Never move company money from a client event: call these from your own server code.
{% endhint %}

Client exports used by ox\_inventory items: `useBillItem`, `useDocument`, `useFlyer`.
