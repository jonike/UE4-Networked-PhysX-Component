Networked PhysX Component
=========================

This project allows players to control pawns that are simulating Physics with PhysX, and provides client-side prediction and reconciliation. It interfaces with the engines INetworkPredictionInterface and is based on the design of the Character Movement Component.

**IMPORTANT: This project is a work-in-progress and NOT COMPLETE**. I'm still working on the general design. There is no smoothing, replay doesn't work properly, there are glitches. Please stop sending me PM's about things that aren't working ;) All in due time...

That said, if you take the code and modify it / improve it - please submit a PR. The aim of the project is to benefit the whole community.

[Unreal Forum Thread](https://forums.unrealengine.com/showthread.php?135955-Networked-Physics-with-PhysX/page2)

TODO
----
* Implement correction smoothing.
* Implement non-local smoothing.
* Use a separate PhysX scene for replay with duplicated static geometry. This will prevent stuttering and collision errors with other non-local pawns. (May require source change).
* Setup for locked and non-locked TimeStep versions of the engine.
* Use new PhysX delegates in 4.15 as well as pre/post Ticks.
* Improve/Add substepping support (?)
* Move to a plugin based format.
* Implement bone-based smoothing for skeletal meshes, so that duplicated collision geometry isn't required for smoothing.

[A pre-compiled version of the initial commit to this repro can be downloaded here.](https://drive.google.com/file/d/0B_FT-hzi26QkbW5WaTgtZGRCUzQ/view?usp=sharing)


License
-------
This project and source are released under the **MIT License.**

TL;DR: do what you want with it, just credit me pls :).


Additional Notes
----------------
Thanks to community members 0lento, Blue Man and OmaManfred for making headway with this problem.
