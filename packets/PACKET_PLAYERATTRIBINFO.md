**MsgPlayerAttribInfo:** This packet is sent from the game server to the game client in newer client versions when the user views the equipment of any player (including themselves). It is used to display all of the characters attributes.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 2071 |
| 4 | UINT32 | Target Identity | 1000000 |
| 8 | UINT32 | Life | 100 |
| 12 | UINT32 | Mana | 1000 |
| 16 | UINT32 | MaximumAttack | 1000 |
| 20 | UINT32 | MinimumAttack | 1000 |
| 24 | UINT32 | Defense | 1000 |
| 28 | UINT32 | MagicAttack | 1000 |
| 32 | UINT32 | MagicDefense | 100 |
| 36 | UINT32 | DodgePercent | 92 |
| 40 | UINT32 | Agility | 20 |
| 44 | UINT32 | Hitrate | 20 |
| 48 | UINT32 | BonusAttackPercent | 20 |
| 52 | UINT32 | BonusMagicPercent | 20 |
| 56 | UINT32 | ReduceDamagePercent | 20 |
| 60 | UINT32 | Unknown60 | 20 |
| 64 | UINT32 | BlessPercent | 20 |
| 68 | UINT32 | CriticalStrikePercent | 20 |
| 72 | UINT32 | SkillCriticalStrikePercent | 20 |
| 76 | UINT32 | ImmunityPercent | 20 |
| 80 | UINT32 | PenetrationPercent | 20 |
| 84 | UINT32 | BlockPercent | 20 |
| 88 | UINT32 | BreakthroughPercent | 20 |
| 92 | UINT32 | CounteractionPercent | 20 |
| 96 | UINT32 | DetoxicationPercent | 20 |
| 100 | UINT32 | DetoxicationPercent | 20 |
| 104 | UINT32 | FinalAttack | 20 |
| 108 | UINT32 | FinalMagicAttack | 20 |
| 112 | UINT32 | FinalDefense | 20 |
| 116 | UINT32 | FinalMagicDefense | 20 |
| 120 | UINT32 | MetalResistPercent | 20 |
| 124 | UINT32 | WoodResistPercent | 20 |
| 128 | UINT32 | WaterResistPercent | 20 |
| 132 | UINT32 | FireResistPercent | 20 |
| 136 | UINT32 | EarthResistPercent | 20 |
