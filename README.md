# A.A.U.-Black-Site-VR
VR Mod for A.A.U. Black Site

<img width="448" height="442" alt="Adobe" src="https://github.com/user-attachments/assets/e9a790b9-a52c-473c-81b5-149531cf32e4" />


A.A.U BLACK SITE VR  -  VR mod for "A.A.U Black Site"
===============================================================================

Version (test build not fully working).

WHAT IT DOES
------------
* Stereo VR through OpenXR (SteamVR, Meta/Oculus, Virtual Desktop, WMR...).
* First person: your headset is the player's head; the body turns with your head. The left stick
  walks where you look, the right stick snap-turns.
* 6DOF weapon: the gun sits in your right controller and shoots where it points (red laser while
  you hold the right grip). The game's own arms / legs are hidden.
* Cutscenes / vehicles / anything that uses another game camera: you sit at that camera.
* The VR controllers are an Xbox controller for the game (its own gamepad controls).
* HUD and menus are on a screen floating in front of you (see-through around them).

INSTALL
-------
1. BepInEx 5 (5.4.23) is already in the game folder - you have it.
2. Copy the BepInEx folder from this zip into the game folder (merge / overwrite).
3. Start SteamVR (or your OpenXR runtime), then start the game.

CONTROLS (the game's gamepad layout)
------------------------------------
Right trigger ......... fire (RT)            Right grip ........... aim (LT) + red laser
Left trigger .......... player status (Back) Right stick click .... kick (R3)
A ..................... jump                 B .................... crouch
X ..................... reload               Y .................... interact
Right stick left/right  snap turn            Right stick up / down  previous weapon / flashlight
Left grip + X ......... heal                 Left grip + Y ........ next weapon
X + Y together ........ pause (Start)        Left stick click ..... L3
Both stick clicks ..... re-centre
In menus: point the right hand (blue laser) at a menu or at a 3D object in the menu room + trigger
(the dot turns gold on 3D objects). The right stick is also the d-pad. X or A = gamepad A (confirm, at the laser),
B = click where the laser points.

WEAPON ADJUST (live): hold BOTH stick clicks 1.7 s with a weapon in hand.
   hold left grip = grab the gun with the left hand and move / turn it, right stick up/down = size,
   B = default, A = save (per weapon).
LASER ADJUST (live): hold BOTH grips 1.7 s, let go, then
   left grip (hold) = move the yellow start point onto the muzzle, right stick = steer the laser,
   B = default, A = save (per weapon). Bullets follow the laser.
IN-GAME VR SETTINGS:    hold Y + left stick click for 1.7 s.
HAND ADJUST:            hold Y + right stick click for 1.5 s.
Everything is in BepInEx\config\aau.blacksite.vr.cfg ([Controls] = gamepad buttons).

USEFUL SETTINGS
---------------
[UI] HealthOnRightHand = true       (health monitor above the ammo counter on the gun)
[UI] HealthOnRightHandOffset = 0,0.06,0
[Aiming] FlashlightHand = Left       (Left / Right controller, or Head like the flat game)
[Aiming] FlashlightOffset = 0,0,0.05
[Camera] NoLensFlares = true (less smear around lights), NoDistortion = false, NoFogReprojection = false
[View] HeadPitchAims = true          (head up/down tilts the game camera and gun)
[Camera] EyeHeightSmoothing = 10     (lower = steadier eyes while walking)
[Camera] RenderScale = 0.8           (raise for sharper, lower for faster)
[Camera] Performance = Balanced      (Quality / Balanced / Fast)
[General] SnapTurn / SnapTurnAngle

FIRST TEST NOT FULLY WORKING
--------------------------------


Uses Astien's OpenXR bridge (see BepInEx\plugins\AAUVR\LICENSES). Free, non-commercial.
