# Changelog

Every ClashPilot release. Downloads are on the [Releases](../../releases) page and on [pilothouse.gg](https://pilothouse.gg/clash-of-clans-bot/changelog).

## 0.1.3 (2026-09-18)

### Fixed

- Playing several accounts in turn could stall on one village for good. Collecting from the collectors, and looking for an upgrade, a wall batch or a research without finding one, no longer count as something to do: a village with nothing left moves on to the next account, or takes its idle break when it is the only one.
- During the goblin builder and goblin researcher events the builder and laboratory buttons wear a goblin's face, and ClashPilot did not recognise them, so no upgrade, wall or research was started for as long as the event ran. It knows both faces now.
- With the storages full, ClashPilot kept tapping the collectors and got round to nothing else. It now collects at most once every five minutes.

## 0.1.2 (2026-09-18)

### New

- ClashPilot can play several accounts in turn. It works one village until there is nothing left to do, moves on to the next through the game's own account list, and goes round. Each account keeps its own General, Attack and Army settings, so a young village and a maxed one can be farmed quite differently. Set them up on the new Accounts page: read them off the game, name them, and put them in the order you want them played.
- A share of the camps is hard to picture, so the Army page now works in troops too. Type what your camps hold and every troop in the recipe shows how many of it will be trained; type a number of troops instead and the share follows. Balance to 100 % puts the shares back in line when you have been typing counts.
- Before it drops the army, ClashPilot zooms the battle map fully out and moves to the top of it, so the whole base is in view when it picks its spots.

### Fixed

- On big accounts whose troop bar runs off the screen, the troops past the first screenful were not dropped and the bar kept scrolling through the battle. The whole army goes down now, heroes already on the field are left where they are, and a reward offered mid-battle is taken before the rest of the army follows.
- Upgrades were passed over while several upgrades were already running.
- The game now offers a goblin builder for gems the moment your last builder is taken, and that made every upgrade look like it had failed: ClashPilot said the upgrade did not start and left the building alone, though it had started perfectly well.

## 0.1.1 (2026-09-15)

### New

- When you open your village on your phone, ClashPilot steps back instead of tapping at the "another device" message. It closes the game, waits ten minutes, then reloads. Still there? It steps back again. You choose the wait, or turn it off, on the Runtime page.
- A new building the game drops onto other buildings is no longer given up on. ClashPilot picks it up and moves it around until it finds a spot where it fits, then places it.

### Fixed

- With the "Fixed spots" drop pattern, spells now land where the troops march in, towards the base. They used to land a little too high.
- Attacks keep coming as long as any storage has room. The dark elixir storage was not being counted, so a village with full gold and elixir but room for dark elixir sat idle.

## 0.1.0 (2026-09-15)

First release. ClashPilot plays your village on your PC and tells you what it did, in plain words. Every line below is a switch you can turn off.

**In the village**

- Collects your resources.
- Keeps your builders busy with upgrades, and can leave some builders free for you.
- Builds new buildings when you can afford them. Skips the Town Hall if you want it to.
- Starts research whenever the laboratory is free.
- Upgrades walls in batches once a storage is nearly full, spending down to a level you choose.
- Clears obstacles, claims achievements and challenges, and collects the loot cart.

**Army and attack**

- Trains the army from a recipe you choose, with a fallback so a young account always has something to train.
- Attacks bases that hold at least the gold, elixir and dark elixir you ask for, and presses Next only as often as you allow.
- Asks your clan for castle troops before the attack and waits for them.
- Drops the whole army round the base, picks reward cards in the order you set, and reads the stars and the loot when the battle ends.

**Pacing and the Log**

- Takes breaks the way a person does: closes the game and powers the emulator off for a while, then comes back.
- No two taps land in quite the same place or at quite the same moment.
- The Log says what it did, one sentence at a time. Statistics for this session, today, 7 days, 30 days and all time.
