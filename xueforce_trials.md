# The Xueforce Trials:

## Structure:
The Xueforce Trials is a ~2-hour event composed of 5 rounds, each of a different type.

The order of these 5 rounds will be random. Each round will have the same scoring. Disambiguation is always by countback.

The specific rules for each round will be announced 5-10 minutes in advance. As can be seen in each type's description below, the rules can vary for various parameters. This will usually be selected at random but could have manual tweaks.

All rounds except for the variety round will be held on the same track, which will be known beforehand.

Mode/map possibilities of the variety round available in [Appendix B](xueforce_trials_variety_maps.md)

Each track has the following information assigned to it. For the full list of values for each track see the [Appendix A](xueforce_trials_track_vars.md):
- MDH: Maximum distance for a single stint with soft tyres with the heavy kart including one lap of cliff
- MDL: Maximum distance for a single stint with soft tyres with the light kart including one lap of cliff
- TLH: How many laps the hard tyre lasts comfortably with medium kart
- TTH: Average time over said stint
- TLM: How many laps the medium tyre lasts comfortably with medium kart
- TTM: Average time over said stint
- TLS: How many laps the soft tyre lasts comfortably with medium kart
- TTS: Average time over said stint

## Round types
### Type 1: Sprint
 - No tyre changes allowed (alloc of 0 0 0)
 - **Parameter**: one kart class that is forced on everyone (light/heavy/medium)
 - **Parameter**: Distance chosen will be any lap count between MDH\*0.7 and MDL\*1.3, rounded up, uniform distribution
 - **Parameter**: Item boxes will be either on or off
 - [TODO: item policy randomization]

### Type 2: Race
 - **Parameter**: between 0 and 1 compounds of Soft, Medium, Hard will be banned.
 - **Parameter**: Any combination of repetitions of the TLH/TLM/TLS lap counts, the corresponding tyre allocation will be given. Then, the allocation be increased/decreased by a total of no more than 10% of the calculated distance when looking at the TL variables. 
 - Length has to target 28-35 minutes in length when calculated according to the TTH/TTM/TTS times their stint lengths
 - **Parameter**: Either one kart class is banned, or all are allowed
 - **Parameter**: Item boxes will be either on or off
 - [TODO: item policy randomization]

### Type 3: Time Trial
 - No tyre changes allowed
 - **Parameter**: One specific compound will be forced
 - No item boxes
 - One lap only
 - **Parameter**: one class will be banned
 - Each player does one lap on a separate session. The fastest wins.

### Type 4: Marathon
 - **Parameter**: Race length 5-12 laps at random with uniform distribution
 - **Parameter**: Forced kart choice.
 - Item policy: Nitro, items *and* bananas forbidden. One zipper per lap, all given at the start
 - Forced tyre choice of tyre 10 (no degradation).
 - Each player will be given a 5 second gap (by speed penalty to all the others) [unless the lap is too short or too long then blablablablayapyapyapyap]
 - 1/3rd of points are given according each to these laptimes: average, median and worst (ranking of each among all players)
 - No autofinish. Only laps after the first lap will be counted.

### Type 5: Variety (can be battle, soccer, capture the flag, egg hunt...)
 - **Parameter**: length decided by organizer
 - It will never be the first nor the last round in the event.
 - **Parameter**: Random forced venue from pre-selected list, forced choice of tyre 10 (no degradation). Must be different from the current track in all cases.
 - Free choice of kart
 - If an individual ranking can be established, it works as usual.
 - If teams, the below is applied:
    Teams must be as balanced in terms of number of players. After that, the sum of points of each team's players' points must be as close as possible.
    Within each team, the players will be ranked according to their score in the gamemode (in soccer goals, in battle hits, etc.).
    Then, if there is a tie, the highest-ranked player in the championship so far has preference.
    Then, the rankings of each team are interleaved, such that the winning team's first player is 1st, the losing team's first player is second, etc.
    In case the result of the match itself was a tie, the team with the least total points gets preference for the interleaving.

Team scoring example:

Scoring of all rounds: 80 40 20 10

Round 4. Socccer match
- Blue team 3 - Red team 5
  - BLUE: nomagno 1 GOAL
  - BLUE: kimden 2 GOALS
  - RED: Cirno 4 GOALS
  - RED: Rowdy 1 GOAL
  - Blue team ranking: 1. kimden 2. nomagno
  - Red team ranking: 1. Cirno 2. Rowdy

Interleaved: 1. Cirno 2. kimden 3. Rowdy 4. nomagno

Points gain: Cirno +80, kimden +40, Rowdy +20, nomagno +10
