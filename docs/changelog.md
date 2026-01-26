---
aside: true
---
# Changelog

## 2.208, 2.2081

- `binaryVersion`: `46` (2.208), `47` (2.2081)
- new getGJScores20 param: `stat` which orders the requested leaderboard by a statistic
- new updateGJAccSettings20 params: `instagram`, `tiktok`, `discord`, `custom` and the corresponding user keys 58-61
- new getGJGauntlets21 param: `vkey`
- new gauntlets (55-60)
- new song type `2`: CHOMPO
- new game variables (176, 177, 179-181)
- the `Cookie: gd=1` header is not sent in requests anymore, it was probably replaced by the new `dvs=3` parameter that's common for almost all endpoints