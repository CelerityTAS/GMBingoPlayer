This file documents all of the TAS encodings that can be played back as a step in bingo TAS playback.

Some Notes:
Spinner cycles will probably have to be removed.
The issue of theo cutscene length can be avoided with retry.
arb checkpoints have to collect all berries before the end of the checkpoint.
1A-dashless-crossing does not flow into 1A-chasm, unless 1A-chasm is played as as retry followed by "Read, 1A-chasm, RTM"

Some files will need alternates to account for RTM vs previous checkpoint entry. It's assumed for now that those differences will be handled by the TAS handler code, and are not documented here.

Italics entries are proposed/not currently encoded.

Entries marked with a * do not complete the checkpoint

```
Total Encodings Needed
Total Count: 96 (through ridge, a-sides only)
Encoded: 10
Remaining: 86
```

# A-Sides
## Forsaken City
| CP Name | Any% | Fast Berries | Heart/Cassette | FC | Other |
|---------|------|--------------|----------------|----|-------|
| Start | 1A-start.tas |-|-| 1A-ARB-start.tas _(1UP COLLECT)_ | 1a-winged-start.tas, _GRABLESS_, 1A-winged-start, _DASHLESS_ |
| Crossing | 1A-crossing.tas | _TODO_ | 1A-heart-crossing.tas | _TODO_ | 1A-theo-crossing, _GRABLESS_, _DASHLESS_ |
| Chasm | 1A-chasm.tas | _TODO_ | 1A-cassette-chasm.tas*(?) | _TODO_ | 1A-winged-chasm.tas, _GRABLESS_, _DASHLESS_ |

### Extra Files
_winged golden collect_, _progress 3up_

## Old Site
| CP Name | Any% | Fast Berries | Heart/Cassette | FC | Other |
|---------|------|--------------|----------------|----|-------|
| Start | _2a-start.tas_ | _TODO (1up)_ | _2A-heart-start.tas_*, _2A-cassette-start.tas_ | _TODO_ (FC, ARB-only, ) | _GRABLESS_ |
| Intervention | _2a-intervention.tas_ | _TODO_ | - | _TODO_ | _GRABLESS_ |
| Awake | _2a-awake.tas_ | _TODO_ | - | _TODO_ | _GRABLESS_, _THEO_, _POEM_ |

## Celestial Resort
| CP Name | Any% | Fast Berries | Heart/Cassette | FC | Other |
|---------|------|--------------|----------------|----|-------|
| Start | _3a-start.tas_ | _TODO_ | - | _TODO_ | _WINGED-ONLY_, _GRABLESS_
| Huge Mess | SPECIAL CASE | | | | _LETTER IN MESS*_
| Elevator Shaft | _3a-shaft.tas | - | 3a-shaft-cassette.tas | _TODO_ | _GRABLESS_, _DIARY IN SHAFT_, _THEO_
| Presidential Suite | _3a-suite.tas | - | - | _TODO_ | _10/15/20 STUNS_, _10/15/20 STUNS (PROGRESS), _GRABLESS_

### Huge Mess
Huge Mess has enough combinations of play that it deserves its own table. (Not necessarily all of these need to be encoded, but should be recorded here)

| Order | Any% | Fast Berries (books/towels) | Heart | ARB | Grabless |
|-|-|-|-|-|-|
| Chests Books Towels | _3a-mess-any.tas_ | _TODO_ | | _TODO_ | _GRABLESS_
| Chests Towels Books | not present in lockout lol
| Towels Chests Books | _TODO_
| Towels Books Chests | N/A | | 3a-mess-heart.tas |
| Books Towels Chests | _3a-mess-btc.tas_ |
| Books Chests Towels | _3a-mess-bct.tas_ |

### PICO-8
To reduce file count, all PICO-8 encodings should enter from Mess entry and not continue. More options are possible (orb with only 5 berries, complete with only 10, etc.) but omitted for brevity.

| Objective | Any% | FC |
|-|-|-|
| 5 Berries | _pico-5.tas_ | - |
| Old Site | _pico-site.tas_ | _pico-site-5.tas_
| 10 Berries | _pico-10.tas_ | - |
| Orb | _pico-orb.tas_ | _pico-orb-10.tas_ |
| 15 Berries | _pico-15.tas_ | - |
| Complete | _pico-clear.tas_ | _pico-clear-15.tas |

### Golden Ridge
| CP Name | Any% | Fast Berries | Heart/Cassette | FC | Other |
|---------|------|--------------|----------------|----|-------|
| Start | _4a-start.tas_ | _1up_ | _4a-start-cassette.tas_ | _TODO (1up)_ | _GRABLESS_, _GRABLESS-CASSETTE_
| Shrine | _4a-shrine.tas_ | _TODO_ | _4a-shrine-heart.tas_ | _TODO_ | _DASHLESS_ |
| Old Trail | _4a-trail.tas_ | _TODO_ | - | _TODO_ | _WINGED*_
| Cliff Face | _4a-cliff-face.tas_ | - | - | _4a-cliff-face-b1.tas_ _4a-cliff-face-fast-berries.tas_ | _GRABLESS_, _10 SNOWBALLS_, _10 SNOWBALLS (PROGRESS)_

## Mirror Temple
TODO

## Reflection
TODO

## The Summit
TODO

## Core
TODO

## Farewell
TODO

# B-SIDES
TODO
