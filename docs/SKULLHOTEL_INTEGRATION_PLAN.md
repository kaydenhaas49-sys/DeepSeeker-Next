# Skull Hotel integration plan

Audit date: 2026-11-25  
Upstream: https://github.com/JamesHall38/skullhotel.io  
Upstream revision inspected: `a0aa7411f0b5e817e51c3267579b38d58b1c7271`  
Archive: `incoming/skullhotel-source.zip` (Git LFS; 107,374,301 bytes)

## Decision

Use Skull Hotel as a **technical reference and selective code donor**, not as a wholesale game fork. Its visual quality and monster presentation are valuable, but its gameplay is built around a fixed eight-room hotel, whereas DeepSeeker-Next is intended to become a large, custom arena with a monster. Copying the original project unchanged would carry over the wrong level geometry, online services, and desktop packaging.

The upstream itch.io page says no generative AI was used. That is the creator's disclosure, not an independent verification.

## Archive inspection

The GitHub Actions audit inspected the ZIP as data only. It did not run scripts, installers, executables, or project code.

- 427 ZIP entries; 371 files; 124,998,950 bytes expanded.
- 0 unsafe paths, symlinks, encrypted entries, duplicate paths, or extreme compression-ratio entries.
- 25 GLB models, 25 KTX2 textures, and 50 MP3 files, plus source, UI, fonts, image and configuration files.
- The archive includes a root MIT license for the code (Copyright James Hall, 2024).
- The README separately attributes assets to Mixamo, BlenderKit, AudioJungle, and AmbientCG. The archive does not contain per-asset license manifests or enough source identifiers to prove the license for each model, texture, sound, or font.

## What to reuse from the code

All copied MIT-licensed code must retain the upstream copyright and license notice in the relevant distribution.

| Upstream area | Decision | How it fits |
|---|---|---|
| `src/components/Monster/Monster.jsx` and `Animations.jsx` | Adapt selectively | Good reference for GLTF character presentation, animation blending, and model setup. Replace asset paths with assets whose licenses are confirmed. |
| `src/hooks/useMonster.js` | Adapt selectively | A compact Zustand store for monster state, position, rotation, and animation is a useful starting pattern. |
| `src/hooks/useMonsterLogic.js` | Port ideas, not wholesale | Its state transitions, anticipation, chase pacing, retreat, and audio coordination are useful. Separate them from hotel-specific state and coordinates. |
| `src/components/PostProcessing.jsx` | Reuse selected effects | Useful reference for atmosphere, distortion, vignette, and colour treatment. Recheck performance and accessibility in the target scene. |
| `src/utils/audio.js` and positional-audio components | Reuse architecture only | The sound registry, volume handling, and positional audio patterns are useful; replace all sound files until their rights are established. |
| `src/components/Player` | Port controls selectively | First-person movement and controller support are useful references. Replace the hotel grid collision model with arena collision. |
| Progressive model/texture loading hooks | Reuse selectively | Useful for keeping a large 3D scene responsive while assets load. |

## What not to copy

- The fixed hotel map and room/corridor geometry.
- `src/hooks/useGrid.js` as the movement/collision system; its cells encode this hotel's doors, curtains, beds, and corridors.
- `src/hooks/useSimplePathfinding.js` unchanged; its waypoints are hard-coded for the hotel corridor openings and bathroom layout.
- Room-specific enemy triggers and seed tables in `TriggersConditions.jsx`, `Triggers.jsx`, and `levelData.js` unchanged.
- Hotel-only objective interactions, room sequence, guestbook, and tutorial flows unless a new design explicitly needs them.
- Firebase guestbook, bug-report upload, analytics, or Firestore reachability checks. DeepSeeker-Next should remain playable offline and not depend on an external Firebase project.
- Electron/Steam wrapper and its Chromium flags. The upstream Electron main process disables important browser security controls (including sandboxing and web security); it should not be carried into a browser-first project.

## Asset licensing gate

The MIT license in the root covers the project's code; it does not automatically relicense third-party art and audio. The README names suppliers but does not record exact asset IDs, URLs, or per-file license choices.

- AmbientCG states its assets are CC0. An asset can be used after matching the actual file to its AmbientCG source.
- Mixamo's FAQ permits royalty-free use of its characters and animations in games. Confirm that each model/animation actually came from Mixamo and retain the applicable terms.
- BlenderKit/BlendKit has per-item license choices; the specific downloaded item and its selected license must be checked.
- AudioJungle licenses are tied to an end product, and stock items cannot be redistributed as stand-alone stock. Do not copy the MP3s into this public repo until the exact purchase/license for each sound is identified.

Until that evidence exists, **do not redistribute the upstream GLBs, KTX2s, MP3s, fonts, or other bundled art files**. Use assets that we own, create, or can clearly verify as CC0/appropriately licensed. Keep the source ZIP private if third-party asset redistribution rights are uncertain; the current repository is public, so anyone can access its LFS archive.

## Dependency and security gate

The archived lockfile was checked using npm's registry advisory database without installing packages or running lifecycle scripts.

- Full lockfile: 44 advisories (3 critical, 33 high, 6 moderate, 2 low).
- Production dependencies only: 6 advisories (2 critical, 1 high, 3 moderate).
- The full list is in [the archive audit](../audits/SKULLHOTEL_ARCHIVE_AUDIT.md).

These are advisory findings across the resolved dependency tree, not proof that every vulnerable code path is reachable in gameplay. They are still enough to block a blind install or deployment. Create a fresh, minimal manifest for the parts we adopt, choose maintained compatible versions, run a new lockfile audit, and fix remaining findings before shipping. Do not blindly run `npm audit fix --force` against the upstream project.

## Proposed DeepSeeker-Next shape

1. Start with a clean browser-first React + Vite + Three.js + React Three Fiber + Drei + Zustand foundation, with a fresh audited dependency lockfile.
2. Build one large, visually rich arena with authored geometry and explicit collision/navigation data. Do not inherit hotel world coordinates.
3. Port a small monster state machine and animation presentation. Use an arena-specific navigation graph/navmesh so the monster can move around obstacles without hotel-specific waypoint assumptions.
4. Add first-person controls, lighting, post-processing, and positional audio in separate, testable modules.
5. Add hiding spots, objectives, or multiplayer only after the single-arena loop is stable.

## Current state

This is a plan, not a code migration. At the time of this audit, DeepSeeker-Next still contains its existing README, the uploaded LFS archive, and the audit workflow/report; no Skull Hotel gameplay source or media assets have been copied into the application.
