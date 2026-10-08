# Graph Report - .  (2026-10-07)

## Corpus Check
- cluster-only mode — file stats not available

## Summary
- 51 nodes · 56 edges · 9 communities (4 shown, 5 thin omitted)
- Extraction: 96% EXTRACTED · 0% INFERRED · 4% AMBIGUOUS
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `f6608d4f`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_Community 0|Community 0]]
- [[_COMMUNITY_Community 1|Community 1]]
- [[_COMMUNITY_Community 2|Community 2]]
- [[_COMMUNITY_Community 3|Community 3]]
- [[_COMMUNITY_Community 4|Community 4]]
- [[_COMMUNITY_Community 5|Community 5]]
- [[_COMMUNITY_Community 6|Community 6]]
- [[_COMMUNITY_Community 7|Community 7]]
- [[_COMMUNITY_Community 8|Community 8]]

## God Nodes (most connected - your core abstractions)
1. `Hermes Gmail Digest home page` - 14 edges
2. `animate()` - 4 edges
3. `preventDefault()` - 2 edges
4. `preventDefaultForScrollKeys()` - 2 edges
5. `animateLogo()` - 2 edges
6. `startGlitchInterval()` - 2 edges
7. `resizeCanvas()` - 2 edges
8. `compileShader()` - 2 edges
9. `createProgram()` - 2 edges
10. `initStars()` - 2 edges

## Surprising Connections (you probably didn't know these)
- `Hermes Gmail Digest home page` --references--> `Cosmic wind graphic`  [AMBIGUOUS]
  index.html → assets/img/cosmicWind.svg
- `Hermes Gmail Digest home page` --references--> `Image asset of unclear subject`  [AMBIGUOUS]
  index.html → assets/img/Hoshimachi-Suisei.png
- `Hermes Gmail Digest home page` --references--> `Clock number graphic`  [EXTRACTED]
  index.html → assets/img/clockNumber.svg
- `Hermes Gmail Digest home page` --references--> `Disc graphic`  [EXTRACTED]
  index.html → assets/img/disc.svg
- `Hermes Gmail Digest home page` --references--> `Header noise texture`  [EXTRACTED]
  index.html → assets/img/header-noise.png

## Import Cycles
- None detected.

## Communities (9 total, 5 thin omitted)

### Community 0 - "Community 0"
Cohesion: 0.15
Nodes (13): Clock number graphic, Cosmic wind graphic, Disc graphic, Header noise texture, Image asset of unclear subject, Clock hour hand graphic, Hermes Gmail Digest home page, Cronous logo graphic (+5 more)

### Community 1 - "Community 1"
Cohesion: 0.15
Nodes (4): hourHand, logo, minsHand, secondHand

### Community 2 - "Community 2"
Cohesion: 0.18
Nodes (8): canvas2D, canvasWebGL, comets, ctx2D, gl, lastMeteorShowerTime, program, stars

### Community 3 - "Community 3"
Cohesion: 0.50
Nodes (4): animate(), createMeteorShower(), createRandomComet(), drawStars()

## Ambiguous Edges - Review These
- `Hermes Gmail Digest home page` → `Cosmic wind graphic`  [AMBIGUOUS]
  index.html · relation: references
- `Hermes Gmail Digest home page` → `Image asset of unclear subject`  [AMBIGUOUS]
  index.html · relation: references

## Knowledge Gaps
- **24 isolated node(s):** `secondHand`, `minsHand`, `hourHand`, `logo`, `canvas2D` (+19 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **5 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Hermes Gmail Digest home page` and `Cosmic wind graphic`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **What is the exact relationship between `Hermes Gmail Digest home page` and `Image asset of unclear subject`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **Why does `Hermes Gmail Digest home page` connect `Community 0` to `Community 8`?**
  _High betweenness centrality (0.073) - this node is a cross-community bridge._
- **Why does `animate()` connect `Community 3` to `Community 2`?**
  _High betweenness centrality (0.001) - this node is a cross-community bridge._
- **What connects `secondHand`, `minsHand`, `hourHand` to the rest of the system?**
  _24 weakly-connected nodes found - possible documentation gaps or missing edges._