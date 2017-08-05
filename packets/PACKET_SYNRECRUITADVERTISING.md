**MsgSynRecuitAdvertising:** This packet is used to place an advertisement for your guild.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 338 |
| 2 | UINT16 | Packet Identifier | 2225 |
| 4 | UINT32 | Id | 1000001 |
| 8 | STRING(256) | Description | "Join us for cookies!" |
| 264 | UINT64 | Amount | 500000 |
| 272 | UINT16 | IsAutoRecruit | 1 |
| 274 | UINT16 | LevelRequirement | 120 |
| 276 | UINT16 | RebornRequirement | 1 |
| 278 | UINT16 | ClassForbid [Flag] | 0 |
| 280 | UINT16 | GenderForbid [Flag] | 0 |
| 282 | UINT16 | UnknownValue | 0 |

Note: the class/gender forbid is a bit flag and lists professions and genders >NOT< permitted to join through the advertisements.
