# Photos on the site

Every picture lives in `images/`. To swap one, upload a new file with the
**exact same name** — nothing in `index.html` changes.

## Shown directly on the page (projects)

| File | Project |
| --- | --- |
| `cfd-velocity-cruise.png`, `cfd-velocity-aoa10.png`, `cfd-pressure-cruise.png` | NACA 2412 CFD |
| `bike-assembly.jpg`, `bike-frame-fea.png`, `bike-beam-model.png` | Bicycle design |
| `jib-crane-fea.png` | Jib crane |
| `subway-thermal.jpg`, `subway-thermal-camera.jpg` | Subway heat research |
| `bulldozer-robot.jpg`, `bulldozer-detail.jpg` | Bulldozer MK I |
| `robotic-arm.jpg`, `robotic-arm-lab.jpg` | Six-DOF robotic arm |
| `bridge-load-test.jpg`, `bridge-truss.jpg` | Tongue-depressor bridge |

## Behind a click (galleries)

`images/leadership/` — 3 photos, under the IMPACT section
`images/conferences/` — 10 photos, under the Conferences section

Both are collapsed by default. A visitor clicks **Photos from the program** or
**Photos from the conferences** to open the grid, then clicks any thumbnail for
the full-size version. The images don't download until someone opens the
gallery, so the page still loads fast.

To add one: drop the file in the folder, then copy an existing `<figure>` block
inside that gallery's `<div class="gal-grid">` and change the three places the
filename appears (`data-full`, `src`, and the caption).

## Still missing

Three project cards have no photo because those folders were empty:

- **Impulse turbine** — the velocity triangle PNGs you have are broken (labels
  overlapping, triangles collapsed to a flat line). Re-run the MATLAB plot and
  send it.
- **Materials selection** — the Ashby chart from ME 461.
- **Residential design** — the floor plan or a Sizer screenshot.

## Rules

- Lowercase filenames, no spaces. GitHub is case-sensitive; Windows isn't.
  This is the usual reason an image works locally and breaks once published.
- Resize to about 1600px wide before uploading — <https://squoosh.app> is quick.
  Target under 300 KB.
- JPG for photographs, PNG for plots, screenshots and CAD renders.
- Write real `alt` text describing what's in the shot.
