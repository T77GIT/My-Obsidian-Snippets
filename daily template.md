---
publish: false 
---
# <% tp.date.now("dddd, MMMM D, YYYY") %>
< [[daily/<% tp.date.now("YYYY-MM-DD-ddd",-1) %>|Yesterday]]
## Tasks
#### Over Due
```tasks
not done
(due before <% tp.date.now("YYYY-MM-DD") %>) OR (scheduled before <% tp.date.now("YYYY-MM-DD") %>)
```
#### Due Today
```tasks
not done
(due on <% tp.date.now("YYYY-MM-DD") %>) OR (scheduled on <% tp.date.now("YYYY-MM-DD") %>)
```
#### New Today

## Daily Check List
### Start of Day
- [ ] 08:30 - 09:00 Clean desk
- [ ] 08:30 - 09:00 Medicine
- [ ] 08:30 - 09:00 Teeth morning
- [ ] 08:30 - 09:00 Nose rinse
- [ ] 08:30 - 09:00 Swap to ergo keyboard
- [ ] 08:30 - 09:00 YNAB
- Drink water
	- [ ] 09:00 - 09:30 +1 Drink water
	- [ ] 11:00 - 11:30 +1 Drink water 
	- [ ] 13:00 - 13:30 +1 Drink water 
	- [ ] 15:00 - 15:30 +1 Drink water 
	- [ ] 17:00 - 17:30 +1 Drink water 
	- [ ] 19:00 - 19:30 +1 Drink water
- [ ] 09:30 - 10:00 Read Programming Book Chapter
- [ ] Bearable Log
- [ ] Shower
- [ ] Teeth evening
- [ ] Medicine evening
- [ ] Exercise
- [ ] Wash dishes
- [ ] Make bed
- [ ] De-clutter
- [ ] Laundry
- [ ] Wipe counters
<%* const dayOfWeek = moment().isoWeekday(); if ( dayOfWeek < 6 ) { -%>- [ ] 09:00 - 09:30 Check emails
- [ ] 09:00 - 09:30 Check teams
- [ ] 09:00 - 09:30 Check repo for new PRs
- [ ] 09:00 - 09:30 Check meeting schedule, prep, set alarms
- [ ] 09:00 - 09:30 Calendar maintenance
- [ ] 09:30 - 10:00 Create work items
- [ ] 09:30 - 10:00 Check tomorrow's calendar
- [ ] 09:30 - 10:00 Prioritise work items
- [ ] 09:30 - 10:00 Create time blocks for larger tasks
- [ ] 09:30 - 10:00 Update work items<%* } -%> 

## Other Tasks

#### No Due Or Scheduled Date
```tasks
not done
(no due date) AND (no scheduled date)
heading does not include End of Day
heading does not include Start of Day
heading does not include End-of-day
heading does not include End-of-week
heading does not include This Week
path does not include templates/
path does not include Recipes/
```

#### Done Today
```tasks

done on <% tp.date.now("YYYY-MM-DD") %>

```

[[<% tp.date.now("YYYY-MM-DD",+1) %>|Tomorrow]] >
