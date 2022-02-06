# Manage events for `!countdown`-command

## Edit events.json to get started, to add an event: 

1. Add event under "eventDates" (if it doesn't already exists)
2. Add an output for the event under "eventOutputs"
3. (Optional) If you want a tag (shortcut) for the event, add it under "eventTags"


## Example, you want to add Tomorrowland 2022 W1 dates:

1. Under "eventDates", add:
```json
"TML22W1Camp" : "July 14, 2022 11:00:00",
"TML22W1Fest" : "July 15, 2022 12:00:00"
```
2. Under "eventOutputs", add:
```json
"TML22W1": {
  "title": "Tomorrowland Weekend 1",
  "events": [
    {
      "title": "Camping",
      "date": "TML22W1Camp"
    },
    {
      "title": "Festival",
      "date": "TML22W1Fest"
    }
  ]
}
```
3. Under "eventTags", add:
```json
"W1": "TML22W1"
```
This will make it possible to get countdowns for W1 camping and festival just by posting `!countdown w1`

---

*Got any questions, or just want to be part of the community?  
Join here: [TMLDiscord.com/github](https://TMLDiscord.com/github)*