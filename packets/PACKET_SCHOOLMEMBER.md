**MsgSchoolMember:** This packet was implemented in the base implementation of their game and server, but was removed before Conquer Online 1.0 Alpha. The message initializes a guild like system called "Hero School", which contains a list of members focused around rankings. From this system, students can be assigned teachers for "tutoring". It can be assumed that this system was later replaced by the Guide/Apprentice system (see the [[MsgGuide]] packet). 

** Packet Definition: ** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]].

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 53 |
| 2 | UINT16 | Packet Identifier | 2037 |
| 4 | BYTE | [[msgschoolmemberaction|Action]] | 1 |
| 5 | BYTE | Member Count | 1 |
| 6 | STMEMBER_INFO[] | "Set of Members" Info |  |

** STMEMBER_INFO Definition: ** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]].

| Data Type | Description | Example |
|---|---|---|---|
| UINT32 | Member Identity | 1000000 |
| CHAR[16] | Member Name | TestAccount1 |
| CHAR[16] | Mate Name | TestAccount2 |
| BYTE | Member Level | 90 |
| BYTE | Member Profession | 13 |
| UINT16 | Member PK Points | 0 |
| BYTE | Member Nobility Rank | 0 |
| BYTE | [[msgschoolmemberrelation|Member Relation]] | 0 |
| BYTE | Member Status (Offline/Online) | 1 |
| UINT32 | Member Syn Rank | 0 |
