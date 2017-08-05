**MsgQuiz:** Displays the quiz show interface and handles questions and replies from players. 

**Patch 5103:** Contributed by [[http://chained2pvp.com/profile/208-felipevieira/|Felipe Vieira]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 18 + String Lengths |
| 2 | UINT16 | Packet Identifier | 2068 |
| 4 | UINT16 | [[msgquizaction|Action]] | 1 |
| 6 | UINT16 | Param1 (Countdown, Score, Question Num.) | |
| 8 | UINT16 | Param2 (Last Correct Answer, Time Taken, Prize) | |
| 10 | UINT16 | Param3 (Time Per Question, Exp. Awarded, Rank) | |
| 12 | UINT16 | Param4 (First Prize, Time Taken) | |
| 14 | UINT16 | Param5 (Second Prize, Current Score) | |
| 16 | UINT16 | Param6 (Third Prize) | |
| 18 | [[msgnetstringpacker|NetStringPacker]]| Strings | 5 Question Answer1 Answer2 Answer3 Answer4 |
