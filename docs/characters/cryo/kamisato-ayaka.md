---
description: Daughter of the Yashiro Commission's Kamisato Clan. Dignified and elegant, as well as wise and strong.
---

import char from '@site/src/data/characters/Kamisato_Ayaka.json'
import { getSkillName } from '@site/src/utils/skill'

# Kamisato Ayaka

import Image from '@theme/IdealImage'

<Image img={require('/img/characters/gacha/Kamisato_Ayaka.png')} />
<blockquote>{frontMatter.description}</blockquote>

## Resources

* [Ayaka Written Guide](https://keqingmains.com/ayaka/)
* [7 Minute Quick Guide to Ayaka](https://youtu.be/G_gQ0P9s6BU)

## Base Stats

import CharStatsTable from '@site/src/components/char/CharStatsTable'

<CharStatsTable char={char} />

## Attacks

import Skill from '@site/src/components/char/Skill'

<Tabs>
<TabItem value='na' label='Normal Attacks'>
<h3>{getSkillName(char, 'na')}</h3>
<div class='talent-columns'>
<Skill char={char} skill='na' sectionFilter='Normal Attack' />

| String    | Talent 9%           | Frames       | MV/s      | Poise Damage | Impulse Type |
| :-------- | :------------------ | :----------- | :-------- | :----------- | :----------- |
| 1-Hit DMG | 84.01%              | 8            | 630.08%/s | 42.5         | 3            |
| 2-Hit DMG | 89.44%              | 28           | 371.68%/s | 44.1         | 3            |
| 3-Hit DMG | 115.05%             | 56           | 309.11%/s | 55.2         | 3            |
| 4-Hit DMG | 41.61% ×3 (124.83%) | 84 + 91 + 98 | 253.06%/s | 19.68 x3     | 2 x3         |
| 5-Hit DMG | 143.64%             | 136          | 245.72%/s | 74.1         | 7            |

</div>
<div class='talent-columns'>
<Skill char={char} skill='na' sectionFilter='Charged Attack' />

| String             | Talent 9%                     | Frames | MV/s      | Poise Damage | Impulse Type |
| :----------------- | :---------------------------- | :----- | :-------- | :----------- | :----------- |
| Charged Attack DMG | 101.28%×3 (303.84%)           | -      | -         | 40 x3        | 2 x2 + 3     |
| N1C                | 84.01% + 101.28%×3 (387.85%)  | 96     | 242.41%/s | -            | -            |
| N2C                | 173.45% + 101.28%×3 (477.29%) | 115    | 249.02%/s | -            | -            |
| N3C                | 288.5% + 101.28%×3 (592.34%)  | 140    | 253.86%/s | -            | -            |
| N4C                | 413.33% + 101.28%×3 (717.17%) | 171    | 251.64%/s | -            | -            |

</div>
<div class='talent-columns'>
<Skill char={char} skill='na' sectionFilter='Plunging Attack' />

| String          | Talent 9% | Poise Damage | Impulse Type |
| :-------------- | :-------- | :----------- | :----------- |
| Plunge DMG      | 117.46%   | 25           | 2            |
| Low Plunge DMG  | 234.86%   | 100          | 4            |
| High Plunge DMG | 293.36%   | 150          | 7            |

</div>

**Notes**

* Ayaka's charged attacks are the first to work in a special way, as follows: When Ayaka starts her CA:
  1. A hitscan occurs for enemies in a radius around her after the NA is over.
  2. After selecting an enemy (closest target or random?), Ayaka will spawn a gadget that locks onto that enemy and follows them regardless of her normal range.
  3. After a brief period, this gadget will stop following the enemy and do an additional 3 hitscans, one for each hit.
  4. A cut with a hitbox will be spawned for each enemy in range of the hitscans. This cut has a hitbox that can hit multiple enemies, but there is an ICD between each cut doing damage to the same enemy. If an enemy leaves the gadget's range while it is still performing the hitscans, the enemy will not be affected by the remaining hitscans. Conversely, the remaining hitscans will affect any enemy that enters the gadget's range even after it has started.
* Ayaka's charged attack ICDs are separate from her normal attack.
* Apart from being able to reach enemies above Ayaka’s ground level (due to Venti’s lift, or Jean’s CA, etc.), Ayaka’s Charged Attacks can also reach enemies below her ground level.

</TabItem>

<TabItem value='e' label='Skill'>
<h3>{getSkillName(char, 'e')}</h3>
<div class='talent-columns'>
<Skill char={char} skill='e' />

| Type              | Skill     |
| :---------------- | :-------- |
| Skill DMG \(T9%\) | 406.64%   |
| Particles         | 4~5 (1:1) |
| Frames            | 56        |
| GU                | 2B        |
| ICD (hits/timer)  | None      |
| Snapshot          | -         |
| Damage Element    | Cryo      |
| Damage Type       | Skill     |
| CD                | 10s       |
| Poise Damage      | 110       |
| Impulse Type      | 7         |

</div>
</TabItem>

<TabItem value='alt' label='Alternative Sprint'>
<h3>{getSkillName(char, 'alt')}</h3>
<div class='talent-columns'>
<Skill char={char} skill='alt'/>

| Attribute                      | Values |
| :----------------------------- | :----- |
| Activation Stamina Consumption | 10     |
| Stamina Drain                  | 15/s   |
| Infusion Duration              | 5s     |
| Poise Damage                   | 0      |
| Impulse Type                   | 2      |

</div>

**Notes**

* 1A Cryo is applied when Ayaka exits from her sprint.
* This infusion causes Ayaka's attacks to apply 1A Cryo
* Her Alternate Sprint has the same iframes as other characters' normal sprint.

</TabItem>

<TabItem value='q' label='Burst'>
<h3>{getSkillName(char, 'q')}</h3>
<div class='talent-columns'>
<Skill char={char} skill='q'/>

| Type                 | Burst         |
| :------------------- | :------------ |
| Cutting DMG \(T9%\)  | 190.91% \* 19 |
| Bloom DMG \(T9%\)    | 286.36%       |
| Cast Frames          | 95            |
| Energy Frame         | 13            |
| CD Frame             | 2             |
| GU                   | 1A            |
| ICD                  | 3 hits / 2.5s |
| Snapshot             | Snapshot      |
| Damage Element       | Cryo          |
| Damage Type          | Burst         |
| Energy Cost          | 80            |
| Duration             | 5s            |
| CD                   | 20s           |
| Cutting Poise Damage | 30            |
| Cutting Impulse Type | 4             |
| Bloom Poise Damage   | 30            |
| Bloom Impulse Type   | 5             |

</div>

**Notes**

* The whirl generated will stay in place for large enemies and frozen enemies
* **Frostflake Seki no To** pushes away all nearby enemies. The extent to which enemies are pushed away depends on their weights & size.
* **Kamisato Art: Soumetsu** deals 20 ticks of damage
  * 19 ticks of **Cutting DMG** and 1 final tick of **Bloom DMG**

</TabItem>
</Tabs>

## Ascension Passives

import PassivesFull from '@site/src/components/char/PassivesFull'

<PassivesFull char={char} />

## Constellations

import Constellation from '@site/src/components/char/Constellation'

<Tabs>
<TabItem value='c1' label='C1'>
<Constellation char={char} constellation={1} />
</TabItem>

<TabItem value='c2' label='C2'>
<Constellation char={char} constellation={2} />

|         | Poise Damage | Impulse Type |
| :------ | :----------- | :----------- |
| Cutting | 30           | 3            |
| Bloom   | 30           | 5            |

**Notes**

* All three **Frostflake Seki no To** (one from burst and the two from C2) can hit the same target.
* The additional **Frostflake Seki no To** share ICD with the main storm.

</TabItem>

<TabItem value='c3' label='C3'>
<Constellation char={char} constellation={3} />
</TabItem>

<TabItem value='c4' label='C4'>
<Constellation char={char} constellation={4} />
</TabItem>

<TabItem value='c5' label='C5'>
<Constellation char={char} constellation={5} />
</TabItem>

<TabItem value='c6' label='C6'>
<Constellation char={char} constellation={6} />

**Notes**

* This effect is additive with other sources of DMG%.

</TabItem>
</Tabs>

## Full Talent Values

import TalentsFull from '@site/src/components/char/TalentsFull'

<TalentsFull char={char}/>

## Evidence Vault

<Card item={require('../../evidence/characters/cryo/kamisato-ayaka.md')} />