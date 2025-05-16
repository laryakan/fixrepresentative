# Fix Representative
This mod aim to force faction representative spawns. Or maybe you're a modder and don't want to bother about representative relocation ?

## What it does ?
*Works on all valid registered factions since v2 - Vanilla, DLC and mods, as soone as the factions is registered in md.$FactionData*

Each time you start a new game or load one (normally,) an mdscript will run an check if there is any missing faction representative. For example, this can happen if you use a mod that modify sector or cluster, or just if the game messed up and you didnt noticed it before the promotion.
Some factions are less impacted than other. But for faction like Free Families, the representative is randomly placed on a whard, shipyard or equipment dock in FRF sectors, many things can happen that prevent the representative spawn.

This is when this script mod come to rescue you, the ForceReprensentative script dispatch the "Missing Representative Task Force", aka **MRTF**.
They will search for the representative and place it on a station of the targeted faction.

## Technically ?
- The script will check existance of representative.
- If a representative is missing, the script will check if the faction is active.
- Then the script will try to reset HQ location and notify the game that there is a problem.
- If the game don't solve the problem, we take things at hand
- We will search for a big station (wharf, shipyard, equipment dock) to make the representative spawn on
- If none : The script will abort, you have an other problem
- If there is one : We update the default faction HQ location and the script will spawn the representative 
- The script will also create a room for him to sit in.
- Then it will update the game data to let it know that a new representative is here.
- TADA

- github : https://github.com/laryakan/fixrepresentative
- nexus : https://www.nexusmods.com/x4foundations/mods/1702
- nexus user : https://next.nexusmods.com/profile/Laryakan
