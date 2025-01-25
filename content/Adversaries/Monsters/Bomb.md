---
statblock: inline
cssclasses:
  - Folder-6
tags:
  - NPCs
---


```statblock
layout: Fabula Ultima NPC
name: "Bomb"
rank: Soldier #optional
level: 10
species: "elemental"
description: "Born in proximity to wildfires or industrial furnaces, these unstable elementals embody the more destructive qualities of fire."

# Use "typicaltraits:" instead of "traits:" if the profile applies to an entire broad category of beings rather than a specific, one-of-a-kind entity.
typicaltraits: "bright, excitable, scorching, unstable."

DEX: 8
INS: 6
MIG: 8
WLP: 10

HP: 60
MP: 60
DEF: 1
MDEF: 2
initiative: 7 #optional

# Affinities: physical, air, bolt, dark, earth, fire, ice, light, poison. All are optional. Only the listed affinities will appear on the sheet.
earth: VU
fire: AB
ice: VU
poison: IM

# Use the attacks-m section for melee attacks and the attacks-r section for ranged -- these are only different in their icons. Both of these sections are technically optional, but the "Basic Attacks" heading will still appear, so please have at least one!
attacks-m:
  - name: "Flame Belch"
    desc: "**[DEX + WLP] + 1 ~ [HR + 10] fire** damage and the target loses Resistance to fire damage until the end of the bomb's next turn."



# Rules -- this section is optional.
rules: 
  - name: "Detonation"
    desc: "When reduced to 0 HP, the bomb explodes dealing **minor (10) fire** damage to every other creature on the scene. If reduced to 0 Hit Points by **ice** damage, the bomb will not explode."


```
