---
tags:
  - character-classes
  - techno-fantasy-atlas
cssclasses:
  - Folder-2
  - alt-tint
---

[Free Benefits::HP + 5 ▪ martial melee weapons ▪ martial ranged weapons]

## Pilot Skills

### Compression Tech
![[Compression Tech|clean no-t]]

### Flexible Configuration
![[Flexible Configuration|clean no-t]]

### Heart in the Engine
![[Heart in the Engine|clean no-t]]

### Personal Vehicle
![[Personal Vehicle|clean no-t]]

### Strong Grip
![[Strong Grip|clean no-t]]

# A Pilot's Vehicle

A Pilot's **personal vehicle** follows a set of special rules.

> - **Entering** the vehicle during a conflict requires the **Objective** action; normally there is no Check required, but the Game Master may introduce a **Clock** in case of serious dangers or obstacles. If the vehicle is accessible when the conflict begins, characters may enter it **immediately** (during step **2** on page **59** of the **Core Rulebook**).
> - **Leaving** the vehicle doesn't require an action, but during a conflict it can only be done on your turn, **before or after** an action.
> - The vehicle can hold a variable number of human-sized creatures depending on its **frame** and **modules**, but **only its Pilot may drive it**. Additionally, the other passengers **cannot cover creatures** when they perform the **Guard** action.
> - The **maximum number of modules active at the same time** on the vehicle is equal to **[3 + its Pilot's Skill Level in Personal Vehicle]**. The Pilot may freely reassign their vehicle's active and inactive modules outside conflicts.

The standard frames and modules are listed in the upcoming pages. Note that whenever a module's text mentions "you", it is referring to the Pilot that the module's vehicle belongs to.

> **Example:** you might create an armored motorbike by combining the **Steed** frame with the **Heavy Plating** and **Turbo modules**; or create a flying combat armor by combining an **Exoskeleton** frame with the **Aerial**, **Runic Plating**, **Rifle** and **Sword modules**.

### List of Frames

```dataview
TABLE WITHOUT ID file.link AS "Frame",
passengers AS "Passengers",
distance AS "Distance",
description AS ""
FROM #frames
```

> **Important:** "passengers" indicates human-sized creatures transported in addition to the Pilot; "distance" refers to the distance traveled during a **travel day**; remember that the maximum number of total active modules on your vehicle is based on your **Skill Level** in **Personal Vehicle**.

## Armor Modules

While driving a vehicle with an active **armor module**, a Pilot does not have access to the normal contents of their **armor slot**. Instead, that slot is considered occupied by the vehicle's **armor module**. If the vehicle has no active armor modules, the Pilot can keep using their equipped armor as normal.

> - As soon as the Pilot is no longer driving a vehicle with an active **armor module**, they immediately regain access to their normal equipped armor.
> - Armor modules marked with <span class="fu-mar"></span> are considered **martial** armors for the sake of Skills and other effects, and they set the Pilot's Defense and Magic Defense to **fixed scores** (bonuses from shields and other effects still apply). Note that a Pilot can still equip these modules **even if they normally lack the ability** to equip martial armors.

> For instance, a Pilot with the **Guardian** Class can gain the benefits of **Defensive Mastery** while driving a vehicle with an active **Heavy Plating module**; at the same time, that Pilot would not be able to benefit from the **Rogue**'s **Dodge** Skill.

### List of Armor Modules

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + " (" + Cost + "z)** " + DEF + " ~ " + MDEF + choice(contains(file.fields, Initiative), "", " ~ " + Initiative + " init.") + "**" AS "Armor Modules"
FROM #modules/basic
WHERE Type = "Armor"
SORT Cost, Name ASC
```

> **Important:** these benefits **only apply to the Pilot who is driving the vehicle**; the scores granted by the **Heavy**, **Runic**, and **Standard Plating modules** can be extended to passengers through the **Expanded Plating module**.

## Weapon Modules

While driving a vehicle with one or more active **weapon modules**, a Pilot does not have access to the normal contents of their **hand slots**. Instead, those slots are considered occupied by the vehicle's **weapon modules**. If the vehicle has no active weapon modules, the Pilot can keep using their equipped items as normal.

> - As soon as the Pilot is no longer driving a vehicle with active **weapon modules**, they immediately regain access to their normal equipped weapons and shields.
> - Each weapon module counts as a **one-handed** weapon for the sake of character Skills and effects (with the exception of the **Shield module**, which is treated as a shield). When you set up your vehicle's weapon modules, declare which module will occupy your **main hand slot** and which module will occupy your **off-hand slot**.
> - Some weapon modules are complex or cumbersome and prevent you from having other weapon modules (including Shield modules!) active on the same vehicle.

> For instance, an **Axe module** can be used to **Counterattack**, and a **Rifle module** can be used for **Crossfire**.

Because each weapon module is treated as a one-handed weapon, a Pilot driving a vehicle with two active weapon modules that share the same Category benefits from the rules for **two-weapon fighting** - and if they have the **Ambidexterous** Heroic Skill, this can be done with **any** two weapon modules!

### List of Weapon Modules

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + " (" + Cost + "z) " + choice(Type = "Shield","","**" + Accuracy + " ~ " + Damage + " " + DamageType + "**<br>" + Range + " ~ This weapon belongs to the **" + Type + "** Category. ") + Effect AS "Weapon Modules"
FROM #modules/basic
WHERE Type != "Armor"
SORT Type, Cost, Name ASC
```

## Support Modules

Support modules provide a variety of miscellaneous benefits; these benefits often apply to the vehicle's passengers in addition to the Pilot themselves.

> - A vehicle cannot have **two or more active support modules with the same name**.
> - Some support modules are particularly complex or cumbersome and count as **two modules** towards the limit on total active modules.

### List of Support Modules

```dataview
TABLE WITHOUT ID choice(contains(file.tags,"removed"),"~~","") + "<span style='text-transform:uppercase;'>**" + file.link + "**</span>" + choice(Restricted = true, " **(" + Restrictions + ")**","") + choice(contains(file.tags, "removed"), "~~","") + choice(contains(file.tags, "core-rework"), "⋆","") + choice(Martial = true, "<span class='fu-mar'></span>","") + " (" + Cost + "z)<br>" + Quality AS "Support Modules"
FROM #modules/rare
WHERE Type = "Support"
SORT Cost, Name ASC
```




# Heroic Skills

```dataview
LIST
FROM #skills/heroic AND [[]]
SORT file.name ASC
```
