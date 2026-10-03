# Changelog

Every ClashPilot release. Downloads are on the [Releases](../../releases) page and on [pilothouse.gg](https://pilothouse.gg/clash-of-clans-bot/changelog).

## 0.2.1 (2026-10-03)

### New

- A battle can end early, by your rules. On the Attack page you can stop a battle once the damage reaches a percentage you set, a number of seconds after the first troop lands, or when the loot left in the base has not dropped for a while. The first rule to come true ends the battle, and you keep the stars and the loot it has by then. Each rule is off until you set it.
- The army goes down at a player's pace. ClashPilot holds a finger down and runs it along the base, so the troops stream out a few a second, the way you would lay a line of archers. A full army takes half a minute or so. The old bursts of taps, quicker than any thumb, are still there as the Fast pace on the Attack page.
- Two more drop patterns. One side lays the army in a line along one edge of the map, a different edge each attack; Two sides lays lines along two edges, each troop type split between them.
- Your Lab Assistant and Builder's Apprentice are put to work. When one of them is free, ClashPilot puts him on the longest research or upgrade running and ticks "Keep assigned until upgrade is complete", so he stays on it until it is done. It is a switch on the General page.
- Builder Base battles press the 1x fast-forward when it shows, as home battles do.
- The Army page adds up a recipe's spells: a line under the list shows the spell space they take, to compare with your spell factory.

### Fixed

- The Grand Warden could be left in the tray. The tap meant to drop him landed on the ground/air switch at the bottom of his tile, and the tap for his ability flipped it back. Heroes are now dropped from a spot clear of the switch.

### Changed

- ClashPilot scrolls twice as far down the upgrade list to find the walls, for accounts with a very long list.

## 0.2.0 (2026-10-01)

### New

- ClashPilot visits your Builder Base. Once a turn on each account, as soon as the village is open, it sails over, does the jobs you switch on, fights by your rule, and sails back home to carry on. It is all on the new Builder Base page, and it is off until you turn it on there.
- Over there it collects the gold, elixir and gem bubbles, empties the Elixir Cart by the dock, and takes the Clock Tower's free boost whenever the clock shows.
- The Master Builder is kept busy with the game's own suggested upgrades, new buildings are bought when you can afford them, and the Builder Hall is skipped if you want it to be. You can keep a builder free there too.
- The Star Laboratory starts the top research you can afford whenever it is free, and the walls are upgraded in batches once a storage is nearly full, spending down to the share you keep, just as at home.
- Builder Base battles. The army is set to one troop of your choice in every slot, then ClashPilot attacks until the storages are full or for a number of battles you set. In each stage it zooms out, drops everything round the base, fires every troop's ability and uses the hero's ability every time it charges. Stop a battle early after the stars you want, or let it run to the end. The stars, the gold and the trophies are read when the battle is over.
- The Statistics page has a Builder Base bay of its own: battles, gold, trophies and stars, kept apart from your home village's attacks.

### Fixed

- Switching accounts could fail for good after a Town Hall upgrade, or whenever the game drew the account list's cards without their Town Hall line. ClashPilot now knows an account by its picture and its names, whichever way the cards are drawn.
- With gold and elixir both full, the walls spent one storage and then waited two minutes before the other, and the buildings got to the second storage first. A wall batch is now followed by the other storage at once.
- A new building priced in gems could pass for one priced in gold. Gem-priced buildings are left alone now.

## 0.1.5 (2026-09-30)

### Fixed

- On an emulator ClashPilot had never played on before, it stopped at "Connecting" with an error and never started. It starts on a fresh emulator now.
- When the game opened on the Builder Base, ClashPilot took it for your home village. It knows the Builder Base now and sails back home first, and it does the same before it moves on to your next account.
- The goblin builder and the goblin researcher work for gems. With only him free, ClashPilot still tried to give him the job; it now waits for a builder or the laboratory of your own.
- An elixir crystal on the map, right behind the elixir bar, could stop ClashPilot reading your elixir, and while your elixir was low no attack was started. It reads the bar past the crystal now.
- The walls sit at the very bottom of the upgrade list. ClashPilot now scrolls further down to find them on accounts with a long list.

### Changed

- With the "Fixed spots" drop pattern, the troops on the right are dropped a little closer to the base.

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
