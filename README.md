Reballanced and improved Overwatch **4v4 All Heroes** mode.

CODE: 48CYD

Differences from the [original script](https://github.com/domuspopus/overwatch-4v4-all-heroes/blob/48df90949be856888b5e3db5ca1917e87e950997/main.ow) usually used in Overwatch 2:

- All new Overwatch 2 heroes are included.
- Ana can nano herself if no target is selected.
- Hammond can grapple onto thin air.
- Junkrat can ult mid-air.
- D.Va does not have never-ending nukes.
- Several tanks have reduced HP.
- Moira and Roadhog start without an ultimate ready.
- Heroes wont fly too far away from map.

![preview](preview.jpg)

### Configuration:

Anything that isn't a simple setting (e.g. HP of a character) can be turned off by simply disabling workshop rule associated with it. All rules have descriptive names. For instance to disable Ana self ult ability, find a rule named "Hero: Ana (self ult)", tick the checkbox on the side of it and toggle the rule off using the button atop the interface. 

### Changelog:

#### 1.3

- Allow Junkrat to ult in mid-air.
- Fix D.Va having instant ult on re-mech (constant D.Va explosions).
- Re-enable HP/Damage auto-ballancing for 2+ players teams.
- Nerf HP/Damage auto-ballancing (decrease damage multiplier).
- Prevent premature game completion (e.g. entire one team leaving).
- Character ballance changes:
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

- Add team sizes ballancing between rounds.
- Add measures to prevent overly long 1v1s (e.g Moira vs Moira).
- Restrict HP/Damage auto-ballancing only to teams with a single player.
- Improvements to anti-fly rules.
- Decrease ultimate generation rate (280% -> 200%).
- Nerf Moira HP and cooldowns.

#### 1.1

- Add trolling prevention (anti-fly rules).
- Ensure faux abilities are affected by "hacked" etc. status effects.
- Increase Hammond cooldowns.

#### 1.0 (changes compared to original script)

- Initial version.
- Decrease some tank HP (Winston/Orisa/Zarya/Hammond/Roadhog).
- Mildly changed ultimate generation values, cleaned up remnants of original "4v4 Nanoblade" in that regard. 
- Roadhog and Moira spawn with no ult ready initially (but can build it).
- Increase Winston damage.
- Let Ana use ult on herself.
- Let Hammond grapple onto nothing (on the fly creating Mei icicle).
