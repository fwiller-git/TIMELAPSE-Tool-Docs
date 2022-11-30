Limitations
===========
* **Cycles render view is not supported**. Viewport capture will default to solid view while attempting to capture from Cycles render view.
* Capturing from multiple cameras can cause a *significant* performance hit. There is not an official upper bound, but you will run into hitches when it captures, if you use too many
* Some addons trigger a false positive for "modal detection" (necessary to prevent undesired behavior and crashing), and are not compatible with TIMELAPSE Tool. The only one discovered so far is `Substance Painter Live Link <https://xolotlstudio.gumroad.com/l/fTRFN>`_. Solutions are being looked into, but the current fix is to disable these addons while recording with TIMELAPSE Tool
* **Dynamic Topology Sculpting** handles sculpt data in a way that is difficult to capture. Anything sculpted with dyntopo enabled will not be captured (mostly) while in sculpt mode. The data seems to only get updated when the project is saved, so TIMELAPSE Tool will only capture what the sculpt looked like the last time you saved. **Enable the "Experimental Settings" and "Capture Dyntopo" in the addon preferences** to make TIMELAPSE Tool save before every capture while in sculpt mode with dyntopo enabled.
* Undo History is cleared when starting and ending a timelapse recording (This prevents crashes and accidentally undo-ing back into or out of the recording state which would break the timelapse). This is a band-aid fix, and other solutions are currently being looked into.
* Capture Interval has a soft minimum of 0.5 minutes, and a hard minimum of 0.1 minutes (accessible by directly typing the value). This may change in the future through an experimental setting

Known Bugs
----------
* Infinite "Modal Detected" Error if starting a recording in the middle of setting the file path. Currently requires reloading the blend file to start recording again. I suspect this will not be an issue when is_operator_modal becomes available in the blender python api, but alternative solutions are being looked in to
* Error Messages when adding or Removing Cameras while multiple 3D viewports are open.
*  **Multiple Viewports** open at the same time is causing several bugs. These will be addressed in the next hotfix!

.. attention::
    Bugs listed here have been officially reported and will be removed as they are fixed. Please report any you find!