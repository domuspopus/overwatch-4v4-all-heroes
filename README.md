Rebalanced and improved Overwatch **4v4 All Heroes** mode (alias **J-edit**, code 48CYD).

---

Main differences from the [older script](https://github.com/domuspopus/overwatch-4v4-all-heroes/blob/48df90949be856888b5e3db5ca1917e87e950997/main.ow) which is often used in Overwatch custom games:

- All new Overwatch 2 heroes are included.
- Ana can nano herself if no target is selected.
- Hammond can [grapple onto thin air](preview-ball-grapple.gif).
- Junkrat can [ult mid-air](preview-junk-ult.gif).
- D.Va does not have never-ending nukes.
- Heroes wont fly too far away from map.
- Overly tanky characters have reduced HP.
- Lobby balancing between rounds.

![preview](preview.png)

### Mode description

Endless 4v4 Elimination quick rounds on a small flat map. Characters are picked randomly and start with an ultimates ready or a high ultimate charge. Ability cooldowns are largely reduced. Perfectly playable as 1v1, 1v2, 2v2, etc. In case of team size imbalance, the smaller team will have buffed HP and damage.

Mode [workshop.codes](https://workshop.codes/48CYD) page.

### Advanced Configuration

Some features and parameters are defined and can be toggled / tweaked inside `Base: Set global variables` rule. Anything else will probably require you disabling workshop rule associated with it. All rules have descriptive names. For instance to disable anti-air mechanics, find a rule named `Base: Prevent heroes flying away`, tick the checkbox on the side of it and toggle the rule off using the button atop the interface.

### Changelog

#### 1.6 (in-development)

- Add advanced lobby balancing.
    - Make each mechanic a toggleable workshop setting.
    - Put new players into random team (default always prefers first team when sizes are equal).
    - Swap random players when one team wins N rounds in a row.
        - If teams are of the same size - swap sides of 2 random opposing players.
        - If winning team is larger - move 1 random player from larger to smaller team.
        - If winning team is smaller - do nothing.
    - Pause/resume via Interact + Primary + Secondary Fire.
- Buff HP/Damage auto-balancing (increase all multipliers).
- Add a HUD showing exact stats as to how much you are buffed by HP/Damage auto-balancing.
- Character balance changes:
    - Orisa: increase HP.
    - Mei: decrease HP.
- Various fixes.

#### 1.5

- Buff HP/Damage auto-balancing for a team of 1.
- Allow Echo to be affected by some faux abilities and effects (e.g. Ana self-ult, Hammond icicle grapple) when she is duplicating.
- Improve character tips and make all of them show on death and between rounds.
- Allow for ultimate generation during start of the round (via custom workaround).
    - This is due to a limitation of Elimination mode, first ~3 seconds of a round disallow ultimate generation.
    - Currently only important for McCree and Soldier.
- Character balance changes:
    - Soldier: increase starting ult charge %, decrease ult duration.
    - Zarya: increase HP.
    - Lifeweaver: decrease petal plate HP, decrease Tree of Life HP and halve its duration.
    - Winston: increase shield cooldown, decrease shield HP.
    - McCree: require him to land a couple shots to build 100% ult charge.
    - Rein: increase passive ult generation rate.
    - Hammond: slightly increase piledriver damage.
- Include daytime version of the map.
- Add server load debug view (interact + reload).
- Various fixes.

#### 1.4

- Rework Hammond icicle grapple for a more consistent and reliable mechanic.
- Buff Hammond piledriver damage and knockback.
- 1v1 time limit improvements, HUD indication for it.
- Various fixes.

#### 1.3

- Allow Junkrat to ult in mid-air.
- Fix D.Va having instant ult on re-mech (constant D.Va explosions).
- Re-enable HP/Damage auto-balancing for 2+ players teams.
- Nerf HP/Damage auto-balancing (decrease damage multiplier).
- Prevent premature game completion (e.g. entire one team leaving).
- Character balance changes:
    - Soldier: start with some % of ult instead of full, decrease ult duration.
    - Mercy: decrease HP, increase resurrection cooldown.
    - Junkrat: increase mines knockback.
    - Hammond: increase grapple knockback, dont create icicle too close, decrease cooldowns.
    - Zarya: slightly increase HP.
    - Orisa: decrease HP.
    - Roadhog: decrease HP.
    - Widowmaker: decrease ability cooldowns.
- Shorter / better UI messages.
- Increase 1v1 time limit.

#### 1.2

- Add team sizes balancing between rounds.
- Add measures to prevent overly long 1v1s (e.g Moira vs Moira).
- Restrict HP/Damage auto-balancing only to teams with a single player.
- Improvements to anti-fly rules.
- Decrease ultimate generation rate (280% -> 200%).
- Nerf Moira HP and cooldowns.

#### 1.1

- Add trolling prevention (anti-fly rules).
- Ensure faux abilities are affected by "hacked" etc. status effects.
- Increase Hammond cooldowns.

#### 1.0 (changes compared to original script)

- Initial version.
- Decrease some tanks HP (Winston/Orisa/Zarya/Hammond/Roadhog).
- Mildly changed ultimate generation values, cleaned up remnants of original "4v4 Nanoblade" in that regard. 
- Roadhog and Moira spawn with no ult ready initially (but can build it).
- Increase Winston damage.
- Let Ana use ult on herself.
- Let Hammond grapple onto nothing (on the fly creating Mei icicle).
