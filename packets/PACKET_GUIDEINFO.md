**MsgGuideInfo:** This packet is sent between the client and game server. It contains information about a mentor and apprentices for a player. The packet is sent on login if the player has a mentor or when required by the client.

**Patch 5103:** Contributed by [[http://chained2pvp.com/profile/208-felipevieira|Felipe Vieira]] and [[http://www.elitepvpers.com/forum/members/2727696--angelius-.html|Angelius]].

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 80 |
| 2 | UINT16 | Packet Identifier | 2066 |
| 4 | UINT32 | Action Type | 2 |
| 8 | UINT32 | User Identity | 1000000 |
| 12 | UINT32 | Target Identity | 1000001 |
| 16 | UINT32 | Lookface | 571003 |
| 20 | UINT32 | Shared Battle Power | 3 |
| 24 | UINT32 | Hours | 1 |
| 28 | UINT32 | Enroll Date | 20160429 |
| 32 | BYTE | Target Level | 130 |
| 33 | BYTE | Target Profession | 55 |
| 34 | UINT16 | Target Pk Points | 17 |
| 36 | UINT16 | Syndicate Identity | 3 |
| 39 | BYTE | Syndicate Rank | 100 |
| 48 | BYTE | Target Online | 1 |
| 52 | UINT32 | Action Type | 2 |
| 56 | UINT32 | Apprentice Experience | 4654698 |
| 64 | UINT16 | Apprentice Blessing | 12 |
| 66 | UINT16 | Apprentice Composing | 200 |
| 68 | BYTE | String Count | 3 |
| 69 | [[msgnetstringpacker|NetStringPacker]] | Strings | 3 6 Mentor 10 Apprentice 10 MentorWife |

**Removing Mentorship:** Hours == 999999; Field is ignored.\\
Hours == 0; The apprentice record is dropped from the mentor list.\\
Hours > 0; Value is parsed as the number of waiting hours left before the mentor-ship is active.\\

To remove the apprentice from the mentor list you send \\
packet 2065 with ActionType = (ExpelApprentice = 18) followed by\\
packet 2066 with ActionType = (ApprenticeList = 2), and the Hours field set to 0.
