**MsgAccount:** This packet is sent during the client's authentication state. It's sent to the account server so that the password exchange can begin. It contains the account name and server from the client's input.

**Patch 4330:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 54 |
| 2 | UINT16 | Packet Identifier | 1051 |
| 4 | CHAR[16] | Account Name | TestAccount |
| 20 | CHAR[16] | Account Password | RC5(MyPassword) |
| 36 | CHAR[16] | Server Name | Meteor |

**Patch 5165:** Contributed by [[http://chained2pvp.com/user/25-caparzo/|Caparzo]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 276 |
| 2 | UINT16 | Packet Identifier | 1086 |
| 4 | CHAR[16] | Account Name | TestAccount |
| 132 | CHAR[16] | Account Password | RC5(MyPassword) |
| 260 | CHAR[16] | Server Name | Meteor |

**Patch 5635:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 240 |
| 2 | UINT16 | Packet Identifier | 1124 |
| 8 | CHAR[128] | Account Name | TestAccount |
| 136 | CHAR[16] | Server Name | Meteor |
| 226 | SHORT | Unknown Enabled | 0 |
| 228 | UINT32 | Unknown | 0 |

**Notes:** Offsets 4, 152-224, and 232-239 are manually set to zero in the client. Offset 225 is never set, and could contain random data. Unknown is related to ini/oem.ini (Section: AccountSetup, Key: Type). If account type is 1, then an argument from server connect is sent (converted from a string to a long). Source of this value is unknown.
