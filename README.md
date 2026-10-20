# CivNodes map tiles

`tiles/{z}/{x}/{y}.png` contains the map images. `api/config.json` contains their
zoom levels and world bounds. Commit both together so they describe the same map.

Generate updates from the website repository using
`python3 scripts/generate_map.py`; its default output is this local `site/map-data/` checkout.

The website repository's GitHub Pages workflow reads this repo's `main` branch.
After pushing updates here, manually run **Deploy map to GitHub Pages** in
`ColtSaboteur/civnodes-map`, or push a website change. This repo has no workflow.
