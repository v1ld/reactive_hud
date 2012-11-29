Reactive HUD
============

A mod for increased hud reactivity: hud elements display and hide themselves
as needed.

Supported HUD mods
------------------

*  oHud

   Primary Needs and Rads meters show only when close to their
   thresholds.

*  Project Nevada

   Energy Cell usage and Grenade quick select show only if an 
   enhanced vision mode is active or a grenade is being selected.

*  HUD Extended

   Health indicator shows only if any limb's condition is below the
   threshold or armor/helmet condition is below the threshold.

All of these mods are _required_ for Reactive HUD to run.

Requirements
------------

*  [NVSE](http://nvse.silverlock.org/)
*  [iHud](http://newvegas.nexusmods.com/mods/40340)
*  All of the supported mods:
   +   [oHud](http://newvegas.nexusmods.com/mods/44757)
   +   [Project Nevada](http://newvegas.nexusmods.com/mods/40040/)
       (The Core module is all that's required.)
   +   [Hud Extended](http://newvegas.nexusmods.com/mods/38589)
*  [Unified HUD](http://newvegas.nexusmods.com/mods/38961)
   (Not required, makes managing the other huds easier.)

Installation
------------

Drop the Reactive HUD.esp file in your Data directory.

Load it after Hud Extended.esp.  (The other masters are all ESMs and
will load earlier.)

Configuration
-------------

These globals adjust some of the behavior.
*  RHudLimbPercentage (85%): show if any limb < 85% healthy.
*  RHudArmorPercentage (50%): show if armor/helmet < 50% condition.
   (Armor protection degrades below 50%.)
*  RHudWeaponPercentage (75%): show if armor/helmet < 75% condition.
   (Weapon damage degrades below 75%.)
*  RHudHTSPercentage (90%): show if any of hunger, sleep, thirst, or
   rads taken > 90% of first threshold (RHudHTSThreshold).
*  RHudHTSThreshold (400): first threshold for HTS values.  The default
   of 400 is from the jsawyer mod.  Vanilla uses 200.

Globals are stored in your save game, so you'll need to use the console
to change one:
*  Bring up the console with the ~ key.
*  Type in "set _globalVariableName_ to _value_" and hit the Enter key.
*  Exit the console by hitting the ~ key again.
*  Save the game.
