SELECTED TRUSS EDITOR UPDATE

Added editing controls to the SELECTED TRUSS panel:
- Change the selected truss classification.
- Change ply count (1–5).
- Edit top chord width/depth, bottom chord width/depth, and web width/depth in millimetres.
- Apply sizes to the selected truss only, or reset its member sections to the generated defaults.
- Updates are applied to the in-memory model and 3D view; the selected truss's member section data is changed for downstream take-off/model operations.

Important engineering limitation:
- Classification changes label the truss type only; they do not regenerate the web layout.
- Member sizing edits do not by themselves prove structural adequacy. Re-run analysis and have loads, restraints, connections, bracing, timber grade and applicable code checks reviewed by a qualified engineer before construction.
- The editor works on the current generated assembly in the browser session. Save/export the project using the app's project/export workflow if you need to retain changes.

Validation performed:
- JavaScript syntax checks passed for all app JS files.
- Existing heel-joint, end-flush, and eave-clash regression tests passed.
