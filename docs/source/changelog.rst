Changelog
=========

Release Versions
----------------

TIMELAPSE Tool: v1.1.0
^^^^^^^^^^^^^^^^^^^^^^
*Idle Detection (Spring QOL Features)*
  * Feature - Detect Idle has been added as a Capture option. This will allow you to capture a timelapse image only after a change is detected in the project (preventing captures that dont have any changes made). I have found this to vastly improve my experience while recording timelapse footage.
  * Feature - JPEG file format option in the Addon Preferences. Should help with hardrive space issues. (Let me know if you want more options here)
  * Feature - Zero Padding adds zeros before the name of the image (eg: 0001.png). Found in the Addon Preferences
  * Tweak - Camera List operations are now available in other modes. This is useful for seeing the view of the timelapse cameras while in edit or sculpt mode.
  * Tweak - Discord Button added to the Panel (get the quickest addon support there)
  * Tweak - Record Button turns Blue while Recording (should help with any confusion of if it's running)
  * Fixed - Grid disappearing while recording in one of the orthographic orientations
  * Fixed - Capture queue not completing when another capture starts during the process.
  * Fixed - Modal Detection broken in Blender 3.5


TIMELAPSE Tool: v1.0.4
^^^^^^^^^^^^^^^^^^^^^^
*Fixes and Tweaks (Thank you for the Bug Reports!)*
  * Tweak - Interval is now in seconds instead of minutes
  * Tweak - Animate is now disabled by default
  * Tweak - Default Image folder has been changed (from //TLTool_Images to //Timelapse_Images)
  * Fix - Camera Capture not functioning properly when using multiple 3D Viewports (context mismatch)
  * Fix - Error with Adding Timelapse Cameras when using multiple 3D Viewports
  * Fix - Timelapse ID not refreshing when creating a new file
  * Fix - Timelapse ID defaulting to previous ID (discovered when creating a new startup file with Timelapse Tool)
  * Fix - Custom Panel Category name reverting to Default when closing Blender
  * BTS - Full Addon Restructure to allow for faster bug fixing and feature additions. (future updates will not take so long)

TIMELAPSE Tool: v1.0.0
^^^^^^^^^^^^^^^^^^^^^^
*Initial Release*
  * Screenshot Capture
  * Camera Capture
  * Multi-Camera Capture
  * Animated Cameras
  * Shading Lock
  * Video from Sequence