repo: HaniehSotudeh/Portfolio
branch: main
path: (whole repo)

## Last sync
date: 2026-09-20T03:48:25Z
commit: 0455ee59f513 (tree hash reported by the API, not a commit sha)

### Updated in this project (latest)
- Rebuilt all 11 School Project detail pages to match the repo's real Bootstrap layouts: natural image aspect ratios (no forced 4:3 crops or letterboxing), 1320px container, exact column fractions (half-width single images, 2/3/4-up rows, 3+8 and 5+5+2 splits), the 5vh side insets from Project-Detail.css, and source image order and caption placement (below vs. beside the image).
- Hero-adjacent text on all 11 project pages matched to Project-Detail.css + Bootstrap defaults: title 40px weight 500 (Bootstrap h1, was 400); #ProjectDetail 18px Lato regular / line-height 1.5 (was 300 / 1.6); #SoftwareSub 18px regular, no opacity (was 14px 300 @0.75); #ProjectDescription keeps the source's `font-family: Lato light` — a family the repo never registers, so it falls back to the browser default serif exactly as the live site does. Ink colour #060808 per the inline spans.
- Typography realigned to Project-Detail.css: 40px project titles, 18px Lato-light body/details, 18px bold centered image captions.
- Corrected single-image blocks: in the source those columns carry an inline `width:100%` that overrides their `col-md-6`, so the image spans the full row (inside the 5vh inset) with its caption centered below — not half width. Applied to Awareness (Sections, Ground/First Floor Plan, Elevation), Chain (Selected Prototype, Fabrication Team), Digital Clay (Form Finding, Plan view), Flexibility (Design Components, Office Layout), Floating Circles (Selected Design, final), Hypermnesia (both collages), Sparkle (Fabrication Pieces), Virginia Falls (From Design To Fabrication, Molding Strategy), The Container (video, Final Semester Prototype, Frame prototype; Interwoven row keeps its 30vh side insets), ConnectedTo (Final Massing Concept, Program Distribution, Section Perspective).
- Missing repo assets: the repo holds 35 of the 40 files Sparkle.html references — `final.png` (hero) and `final model.png` / `- 2` / `- 3` / `- 4` are referenced but not committed (the live site must serve them from a deployed copy outside git). Sparkle's hero and its restored "Fabricated Model" 4-up now use drop-in <image-slot> placeholders pointing at those exact source paths, so the real files can be added without touching layout. Comfort Zone's cover (`1-new.png`) is likewise absent and still uses a substitute.

### Updated previously
- Fixed a direct-edit regression in ConnectedTo.dc.html that nested captionless images inside a "has title" check, hiding several images (ct-7, water/resized shots, Untitled Recovered pair). Verified full content parity against ConnectedTo.html in the repo.
- Fixed Parametric Fun grid (tiles had no height; aspect-ratio moved onto the container).
- Footer sitewide: black bar, LinkedIn/Email/Instagram icons only, credit reads "Designed by Hanieh Sotudeh and Claude Design".
- School Projects grid + all 11 project detail pages converted from dark to white theme; sticky sidebar removed on detail pages.


### Updated in this project
- Imported the full site into this project as matching dark-theme DC pages: index.html (index), School Projects.dc.html (editorial grid, was Projects.html), Parametric Fun.dc.html, and 11 individual project detail pages (Awareness, Chain, ComfortZone, ConnectedTo, DigitalClay, Flexibility, FloatingCircles, Hypermnesia, Sparkle, TheContainerAndTheContained, VirginiaFalls).
- Copied all real project imagery from assets/img/Project/* and assets/img/Parametric Fun/Content into this project, preserving folder structure.
- Detail pages use the same sticky-sidebar + scroll-reveal layout established on Professional Work/CV; nav now links between these local files instead of the live site.
- Everyday Acoustics keeps its original external link (https://www.everydayacoustics.com/) since it's hosted off-site.
- Note: a couple of source images referenced by the original HTML (Comfort Zone's "1-new.png", Sparkle's "final.png") are missing from the current repo tree — substituted with the closest existing image as a stand-in cover.

## Screen map
| Screen (this project) | Repo files it was built from |
|---|---|
| index.html | index.html |
| School Projects.dc.html | Projects.html, Portfolio-with-Category-switcher.css |
| Parametric Fun.dc.html | ParametricFun.html |
| Awareness.dc.html | Awareness.html + assets/img/Project/Awareness/* |
| Chain.dc.html | Chain.html + assets/img/Project/Chain/* |
| ComfortZone.dc.html | ComfortZone.html + assets/img/Project/Comfort Zone/* |
| ConnectedTo.dc.html | ConnectedTo.html + assets/img/Project/ConnectedTo/* |
| DigitalClay.dc.html | DigitalClay.html + assets/img/Project/Digital Clay/* |
| Flexibility.dc.html | Flexibility.html + assets/img/Project/Flexibility/* |
| FloatingCircles.dc.html | FloatingCircles.html + assets/img/Project/Floating Circles/* |
| Hypermnesia.dc.html | Hypermnesia.html + assets/img/Project/Hypermnesia/* |
| Sparkle.dc.html | Sparkle.html + assets/img/Project/Sparkle/* |
| TheContainerAndTheContained.dc.html | TheContainerAndTheContained.html + assets/img/Project/TheContainerAndTheContained/* |
| VirginiaFalls.dc.html | VirginiaFalls.html + assets/img/Project/Virginia Falls/* |
| Professional Work.dc.html, CV.dc.html | (private, not from repo — nav updated to link to the new local pages) |

Not imported (BerlinHolocaust.html / LUmbracle.html look like abandoned/duplicate drafts of the same content — ask before building if wanted).
