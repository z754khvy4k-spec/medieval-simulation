# Medieval Simulation V5 — Spatial Economy

V5 extends the V4 simulation into a geography-aware economic system.

## New economic layer
- Five local markets / regions.
- Physical inventories are local to regions.
- Businesses compare local input prices against delivered costs from other regions.
- Carts move goods between regions over multiple simulation days.
- Transport consumes cash and time and depends on distance.
- Regional price clearing means shortages and surpluses create spatial price differentials.
- Merchants / firms can arbitrage when landed costs justify trade.
- Grain -> flour -> bread is a physical multi-stage chain.
- Wool -> cloth, iron -> tools, wood -> fuel are additional chains.
- Farm output depends on season, weather and tool availability.
- Weather events include drought, storm, frost, flood, rain, dry and wind.
- Goods have spoilage rates; bread and other perishables decay.
- Households pay recurring rent and can borrow emergency credit.
- Household debt and business debt accrue interest.
- Firms can become insolvent and go bankrupt, releasing labor.
- Wages vary with local output prices and occupation.
- Businesses hire/fire based on expected contribution margins.
- Food shortages cause hunger, physiological damage, starvation duration and mortality.
- Limited NPC market knowledge persists with decay.

## World layer
- Real-time Three.js world with procedural buildings, fields, roads, river, town square and trees.
- Carts are rendered and move along the world as simulated trade occurs.
- Business locations are tied to their economic region.
- Clickable buildings and households open detailed inspectors.

## Important implementation note
The 3D models are lightweight procedural primitives so the browser version remains deployable and fast. The included OBJ prototypes can later be replaced by higher-fidelity Blender assets without changing the economic simulation API.

## Deployment
Upload `index.html`, `manifest.webmanifest`, `sw.js`, and `README.md` to the repository root. GitHub Pages can serve the app. The current renderer imports Three.js from jsDelivr, so an internet connection is required.
