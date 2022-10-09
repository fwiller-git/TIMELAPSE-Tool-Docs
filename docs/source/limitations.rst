Limitations
===========
* Capturing from multiple cameras can cause a *significant* performance hit. There is not an official upper bound, but you will run into hitches when it captures if you use too many
* Some addons trigger a false positive for "modal detection" (necessary to prevent undesired behavior and crashing), and are not compatible with TIMELAPSE Tool. The only one discovered so far is `Substance Painter Live Link <https://xolotlstudio.gumroad.com/l/fTRFN>`_. Solutions are being looked into, but the current fix is to disable these addons while recording with TIMELAPSE Tool
* **Dynamic Topology Sculpting** handles sculpt data in a way that is difficult to capture. Anything sculpted with dyntopo enabled will not be captured (mostly) while in sculpt mode. The data seems to only get updated when the project is saved, so TIMELAPSE Tool will only capture what the sculpt looked like the last time you saved. **Enable the "Experimental Settings" and "Capture Dyntopo" in the addon preferences** to make TIMELAPSE Tool save before every capture while in sculpt mode with dyntopo enabled.

Known Bugs
----------
* None so far (Please report any you find)...

.. note::
    Bugs listed here have been officially reported and will be removed as they are fixed

