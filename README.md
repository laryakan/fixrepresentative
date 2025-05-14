# Fix Representative
In some case, modders forget or the game bugs. This mod aim to force Faction representatives spawn or fix them for some mods.

## What it does ?
*For the time being, only work on FRF Representative as a proof of concept*

Each time you start a new game, an mdscript will run an check if there is any missing faction representative. For example, this can happen if you use a mod that modify sector or cluster.
Some factions are less impacted than other. But for other, like Free Families, the representative is randomly placed on a whard, shipyard or equipment dock in FRF sectors : If a mod or a bug mess up with FRF sector, the representative could not spawn.

Then, the ForceReprensentative script dispatch the "Missing Representative Task Force", aka **MRTF**.
They will search for the representative and place it on a random station of the targ faction.

## Technically ?
The script will check existance of representative.
If a representative is missing, the script will check if the station is active.
Then it will check if there is an eligible station for the representative to land on.
If none, the script will abort. But if there is one, the script will reset the default HQ settings for this factions, create the representative, create a room for him to sit in and place him inside it.

For the time being, the first version on this mod only check the FRF representative, but other factions can easily be check, including small factions.
