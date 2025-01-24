> [!info|clean no-t flush]
> ### Psychic Gifts

> [!list|inline no-icon] Brainwave Clock
> - [ ] |
> - [ ] |
> - [ ] |
> - [ ] 

> [!list|rules no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + "** ~ " +  trigger + "...<br>" + effect
>
FROM outgoing([[]])
WHERE contains(file.tags, "psychic-gifts")
SORT file.name asc
>```
