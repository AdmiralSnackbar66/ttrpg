## Pathfinder 2e example

Below is a Dataview query that returns all creatures with the type "Plant" with a Level between 5 and 10.

```dataview
TABLE level as "Level", hp as "HP" from "monsters/Pathfinder 2e"
where contains(file.tags, "pf2e/creature/type/plant") and
level >5 and level <10
```


## 5e example

Below is a Dataview query that returns all creatures with the type "Plant" with a CR between 7 and 10. Feel free to adjust it to your specifications!

```dataview
table cr as "CR", type as "Type", source as "Source", url as "URL" from "monsters"
where contains(lower(type),"plant") and cr <10 and cr>7
sort cr DESC
```

