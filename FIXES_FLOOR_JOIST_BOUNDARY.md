# Floor joist boundary fix

- Floor joists are now clipped to each closed `FLOOR` LWPOLYLINE boundary.
- Each joist line is intersected with polygon edges; paired intersections define the valid inside-floor spans.
- Concave floor outlines can produce multiple in-boundary joist segments, rather than full bounding-box joists projecting beyond walls.
- Wall framing generation is unchanged.
- Added `app/test-cad-floor-clipping-v3.mjs` to check that rectangular-floor joist endpoints remain within the CAD boundary.
- Verification: floor clipping test and CAD-layer generation test passed. Full `test-dxf.mjs` remains dependent on its fixture containing the required `TRUSSES` layer.
- Geometry is schematic and still requires engineering review.
