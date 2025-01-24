> [!info|clean no-t flush]
> ### Spells

> [!list|inline no-icon] Ritual Disciplines
> - [ ] Ritualism
> - [ ] Arcanism
> - [ ] Chimerism
> - [ ] Elementalism
> - [ ] Entropism
> - [ ] Spiritism
> 
> %%**Restrictions:**%%

> [!list|spells no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + choice(contains(file.tags, "core-reworks"), "⋆", "") + choice(contains(file.tags, "spells/offensive"), "<span class='fu-off'></span>", "") + "** ~ **" + cost + " MP** ~ **" + target + "** ~ **" + duration + "**<br>" + effect
>
FROM outgoing([[]])
WHERE contains(file.tags, "spells")
SORT file.name asc
>```
