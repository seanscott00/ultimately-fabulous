---
tags:
  - character-classes
  - core-rulebook
cssclasses:
  - Folder-2
  - alt-tint
---

[Free Benefits::MP +5 ▪ Ritualism]

## Entropist Skills

### Absorb MP

![[Absorb MP|clean no-t]]

### Entropic Magic

![[Entropic Magic|clean no-t]]

### Lucky Seven

![[Lucky Seven|clean no-t]]

### Ritual Entropism

![[Ritual Entropism|clean no-t]]

### Stolen Time

![[Stolen Time|clean no-t]]

# Entropist Spells

> [!list|spells no-title]
> ```dataview
LIST WITHOUT ID "**" + file.link + choice(contains(file.tags, "core-reworks"), "⋆", "") + choice(contains(file.tags, "spells/offensive"), "<span class='fu-off'></span>", "") + "** ~ **" + cost + " MP** ~ **" + target + "** ~ **" + duration + "**<br>" + effect
>
> FROM #spells and #entropist
> SORT file.name asc
> ```

# Heroic Skills

```dataview
LIST
FROM #skills/heroic AND [[]]
SORT file.name ASC
```
