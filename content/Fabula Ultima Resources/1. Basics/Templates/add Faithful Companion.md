---
FullName: none
Traits: four traits
Level: 1
PartnerLevel: 5
Species: species
DEX: 8
INS: 8
MIG: 8
WLP: 8
HP: 0
MP: 0
DEF: "8"
MDEF: "8"
freeHP: 0
freeMP: 0
Physical: none
Air: none
Bolt: none
Dark: none
Earth: none
Fire: none
Ice: none
Light: none
Poison: none
tags:
  - npc-companions
cssclasses:
  - Folder-4
---

> [!infobox]
> 
> ![[avatar.png]]
> 
> ### Faithful Companion
>
> ###### *`=this.Traits`*
> 
> |Level|5 (SL`=this.Level`)|Species|`=this.Species`|
> |:-|:-|:-|:-|
> | **DEX** | d`=this.DEX` | **DEF** | `=this.DEF` |
> | **INS** | d`=this.INS` | **M. DEF** | `=this.MDEF` |
> | **MIG** | d`=this.MIG` |
> | **WLP** | d`=this.WLP` |
>
> | HP | MP |
> | :-: | :-: |
> | `=round(this.Level * this.MIG + this.PartnerLevel/2-0.5)` ~ `=round(round(this.Level * this.MIG + this.PartnerLevel/2-0.5)/2-0.5,0)` | `=this.WLP*5` |
> 
> | | | |
> | :-: | :-: | :-: |
> | `=choice(this.Physical = "none", "<span class='fu-phys-s'></span>", "<span class='fu-phys'></span> " + this.Physical)` | `=choice(this.Air = "none", "<span class='fu-air-s'></span>", "<span class='fu-air'></span> " + this.Air)` | `=choice(this.Bolt = "none", "<span class='fu-bolt-s'></span>", "<span class='fu-bolt'></span> " + this.Bolt)` |
> | `=choice(this.Dark = "none", "<span class='fu-dark-s'></span>", "<span class='fu-dark'></span> " + this.Dark)` | `=choice(this.Earth = "none", "<span class='fu-earth-s'></span>", "<span class='fu-earth'></span> " + this.Earth)` | `=choice(this.Fire = "none", "<span class='fu-fire-s'></span>", "<span class='fu-fire'></span> " + this.Fire)` |
> | `=choice(this.Ice = "none", "<span class='fu-ice-s'></span>", "<span class='fu-ice'></span> " + this.Ice)` | `=choice(this.Light = "none", "<span class='fu-light-s'></span>", "<span class='fu-light'></span> " + this.Light)` | `=choice(this.Poison = "none", "<span class='fu-psn-s'></span>", "<span class='fu-psn'></span> " + this.Poison)` |
> 

> [!info|clean no-t flush]
> ## Description

_This creature **does not level up**, can have a **maximum of two basic attacks**, gains a bonus equal to **[`=this.Level`]** to Accuracy Checks and Magic Checks, and their maximum Hit Points are equal to **[`=round(this.Level * this.MIG + this.PartnerLevel/2-0.5)`]**._

> [!list|melee clean no-title flush]
> ### Basic Attacks
> 
> - **Melee Attack ~ [Check] +`=this.Level` ~ [damage formula] type** damage, followed by any special rule or effect.

> [!list|ranged clean no-title flush]
> - **Ranged Attack ~ [Check] +`=this.Level` ~ [damage formula] type** damage, followed by any special rule or effect.

> [!list|spells clean no-title flush]
> ### Spells
> - **Spell name (<span class="fu-off"></span> if offensive) ~ [Check] +`=this.Level` ~ Cost ~ Target ~ Duration.**  
Effect.

> [!list|skills clean no-title flush]
> ### Other Actions
> - **Action name** ~ See the rules for **writing an effect**.

> [!list|rules clean no-title flush]
> ### Special Rules
> - **Rule name** ~ See the rules for **writing an effect**.
