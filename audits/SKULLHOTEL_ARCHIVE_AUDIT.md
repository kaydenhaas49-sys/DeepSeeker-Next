# Skull Hotel source archive audit

Inspection method: read-only ZIP metadata and bounded text-file reads. No project scripts, installers, or binaries were executed.

- Archive bytes: 107,374,301
- SHA-256 is recorded by Git LFS (see repository pointer); this report does not copy secret values.

## Archive structure
- Entries: 427 (371 files)
- Declared expanded size: 124,998,950 bytes
- Unsafe paths: 0
- Symlinks: 0
- Encrypted entries: 0
- Duplicate paths: 0
- Compression ratios above 200:1: 0

## File types

| Extension | Count |
|---|---:|
| .jsx | 90 |
| .mp3 | 50 |
| .js | 49 |
| .json | 33 |
| .glb | 25 |
| .ktx2 | 25 |
| .jpg | 24 |
| .svg | 23 |
| .css | 18 |
| .png | 9 |
| [no extension] | 3 |
| .yml | 3 |
| .ttf | 3 |
| .webp | 3 |
| .wasm | 2 |
| .example | 1 |
| .md | 1 |
| .manifest | 1 |
| .rules | 1 |
| .html | 1 |
| .otf | 1 |
| .ico | 1 |
| .webmanifest | 1 |
| .ini | 1 |
| .txt | 1 |
| .xml | 1 |

## Largest files

| Path | Expanded bytes |
|---|---:|
| `skullhotel.io-master/public/textures/floor/floor_roughness.jpg` | 16,728,805 |
| `skullhotel.io-master/public/models/monster.glb` | 16,367,540 |
| `skullhotel.io-master/public/textures/floor/floor_color.jpg` | 5,626,729 |
| `skullhotel.io-master/public/models/monster-opt.glb` | 5,504,080 |
| `skullhotel.io-master/public/textures/carpet/carpet_color.jpg` | 5,202,460 |
| `skullhotel.io-master/public/textures/bathroom/baked_bathroom.jpg` | 4,626,571 |
| `skullhotel.io-master/public/textures/food/baked_food.jpg` | 3,470,574 |
| `skullhotel.io-master/public/textures/livingroom/baked_livingroom.jpg` | 3,460,759 |
| `skullhotel.io-master/public/textures/bathroom/roughness_bathroom.jpg` | 3,242,661 |
| `skullhotel.io-master/public/textures/walls/walls_color.jpg` | 3,179,623 |
| `skullhotel.io-master/public/EB_Garamond_Regular.json` | 2,550,491 |
| `skullhotel.io-master/public/models/objectives/bedsheets.glb` | 2,462,000 |
| `skullhotel.io-master/public/textures/bedroom/roughness_bedroom.jpg` | 2,402,634 |
| `skullhotel.io-master/public/textures/bedroom/baked_bedroom.jpg` | 2,362,730 |
| `skullhotel.io-master/public/sounds/ambiant2.mp3` | 2,291,754 |
| `skullhotel.io-master/public/textures/livingroom/roughness_livingroom.jpg` | 2,250,218 |
| `skullhotel.io-master/public/textures/carpet/carpet_roughness.jpg` | 2,099,628 |
| `skullhotel.io-master/public/textures/reception/reception_color.jpg` | 1,575,460 |
| `skullhotel.io-master/public/textures/fabric/fabric_color.jpg` | 1,561,134 |
| `skullhotel.io-master/public/textures/reception/reception_light_uastc.ktx2` | 1,398,656 |
| `skullhotel.io-master/public/models/doors/curtain.glb` | 1,364,012 |
| `skullhotel.io-master/public/sounds/tense.mp3` | 1,328,022 |
| `skullhotel.io-master/public/textures/reception/reception_roughness.jpg` | 1,285,618 |
| `skullhotel.io-master/public/textures/walls/walls_roughness.jpg` | 1,282,590 |
| `skullhotel.io-master/public/models/wooden_mannequin.glb` | 1,123,080 |
| `skullhotel.io-master/public/capsule_1200x675.png` | 883,349 |
| `skullhotel.io-master/public/sounds/ambiant1.mp3` | 880,984 |
| `skullhotel.io-master/public/textures/carpet/carpet_color_etc1s.ktx2` | 853,511 |
| `skullhotel.io-master/public/textures/bathroom/light_bathroom.jpg` | 853,305 |
| `skullhotel.io-master/public/models/objectives/tasks.glb` | 821,604 |

## Package manifests
### `skullhotel.io-master/package.json`
- Package: skullhotel 1.1.0
- Declared license: MIT
- Runtime dependencies: 15
- Development dependencies: 9
- Scripts (not executed): build, build:electron, build:firebase, build:itch, build:steam, build:steam-dist, dev, electron, fix-paths, preview

**Runtime dependencies**

- `@gsap/react`: `^2.1.2`
- `@react-spring/three`: `^10.0.3`
- `@react-three/drei`: `^9.122.0`
- `@react-three/fiber`: `^8.18.0`
- `@react-three/postprocessing`: `^2.16.7`
- `@types/three`: `^0.180.0`
- `firebase`: `^12.4.0`
- `leva`: `^0.9.35`
- `postprocessing`: `^6.37.8`
- `react`: `^18.3.1`
- `react-dom`: `^18.3.1`
- `react-icons`: `^5.5.0`
- `steamworks.js`: `^0.4.0`
- `three`: `^0.180.0`
- `zustand`: `^5.0.8`

**Development dependencies**

- `@eslint/js`: `^9.38.0`
- `@vitejs/plugin-react`: `^4.7.0`
- `electron`: `^39.0.0`
- `electron-builder`: `^26.0.12`
- `eslint`: `^9.38.0`
- `eslint-plugin-react`: `^7.37.5`
- `eslint-plugin-react-hooks`: `^7.0.1`
- `globals`: `^16.4.0`
- `vite`: `^6.4.1`

## Lockfile

- `skullhotel.io-master/package-lock.json`: lockfileVersion 3
- Package records: 850

## License and attribution files

- `skullhotel.io-master/LICENSE` (1067 characters)

## README asset and attribution references

- Line 2: <img src="./assets/main.jpg" alt="Skull Hotel" style="margin-bottom: 20px;">
- Line 39: <img src="./assets/grid-visualization.png" alt="Room Grid Visualization">
- Line 44: - **Mixamo**: Character model and animations
- Line 45: - **BlenderKit**: 3D assets
- Line 46: - **AudioJungle**: Sound effects
- Line 47: - **AmbientCG**: Textures and materials

## Configuration and secret-pattern screening

- Environment-file paths: `skullhotel.io-master/.env.example`
- No matches for the limited high-signal patterns in bounded text files.
- This is a heuristic screen, not a guarantee that the archive contains no secrets.

## Safety checks

- Unsafe ZIP paths: none found
- Symlink entries: none found
- Encrypted entries: none found
- Extreme compression ratios: none found
- No archive code or install scripts were run.

