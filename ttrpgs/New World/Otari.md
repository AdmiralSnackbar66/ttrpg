---
type: place
faction: 
location: 
world: New World
campaign: New World
date: 2023-01-15
description: ""
race: 
gender: 
class: 
---
# [[Otari]]

Otari is a seaside village.

```dataview
table description as "Description" from "ttrpgs/New World"
WHERE contains(type,"NPC") or contains(type,"faction") and contains(location,"Otari")
SORT file.name ASC
```
