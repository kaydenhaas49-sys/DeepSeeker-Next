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

## npm advisory check (lockfile only)

- npm exit code: 1
- Vulnerabilities: {"critical": 3, "high": 33, "info": 0, "low": 2, "moderate": 6, "total": 44}
- `@babel/core`: low — @babel/core: Arbitrary File Read via sourceMappingURL Comment
- `@electron/node-gyp`: high — make-fetch-happen, tar
- `@electron/rebuild`: high — @electron/node-gyp, tar
- `@grpc/grpc-js`: high — @grpc/grpc-js: A malformed request can cause a server crash, @grpc/grpc-js: An incoming malformed compressed message can cause a client or server crash, @grpc/grpc-js: In certain configurations, getAuthContext can return unauthorized certificates as though they were authorized
- `@humanfs/node`: moderate — humanfs: Recursive copy follows symlinked files and copies data from outside the source tree
- `@isaacs/brace-expansion`: high — @isaacs/brace-expansion has Uncontrolled Resource Consumption
- `@protobufjs/utf8`: moderate — protobufjs has overlong UTF-8 decoding
- `@tootallnate/once`: low — @tootallnate/once vulnerable to Incorrect Control Flow Scoping
- `@xmldom/xmldom`: high — xmldom: XML injection via unsafe CDATA serialization allows attacker-controlled markup insertion, xmldom: Uncontrolled recursion in XML serialization leads to DoS, xmldom has XML injection through unvalidated DocumentType serialization
- `ajv`: moderate — ajv has ReDoS when using `$data` option
- `app-builder-lib`: high — @electron/rebuild, electron-updater: Uncontrolled search path elements within `AppImage` built by `app-builder-lib`, builder-util
- `baseline-browser-mapping`: moderate — baseline-browser-mapping process termination on invalid input causes denial of service
- `brace-expansion`: high — brace-expansion: Zero-step sequence causes process hang and memory exhaustion, brace-expansion: Zero-step sequence causes process hang and memory exhaustion, brace-expansion: DoS via exponential-time expansion of consecutive non-expanding {} groups
- `browserslist`: high — Browserslist: Unbounded memory growth (no cache eviction) via distinct query results, leading to eventual OOM, Browserslist: Uncaught crash / prototype write via untrusted browserslist-stats.json custom stats (normalizeStats)
- `builder-util`: high — builder-util-runtime
- `builder-util-runtime`: high — electron-updater: Cross-origin redirect leaks `PRIVATE-TOKEN` and mixed-case `Authorization` credentials in `builder-util-runtime`
- `cacache`: high — tar
- `colord`: moderate — Colord: Slow rejection of oversized malformed color strings
- `dmg-builder`: high — app-builder-lib, builder-util, builder-util-runtime
- `electron`: high — Electron: AppleScript injection in app.moveToApplicationsFolder on macOS, Electron: Service worker can spoof executeJavaScript IPC replies, Electron: Incorrect origin passed to permission request handler for iframe requests
- `electron-builder`: high — app-builder-lib, builder-util, builder-util-runtime
- `electron-builder-squirrel-windows`: high — app-builder-lib, builder-util
- `electron-publish`: high — builder-util, builder-util-runtime
- `extract-zip`: high — extract-zip unvalidated symlink path traversal, extract-zip allows arbitrary file writes through symlink archive entries
- `fflate`: moderate — fflate unzipSync can enter an infinite loop when parsing malformed ZIP64 archives, fflate unzipSync can enter an infinite loop when parsing malformed ZIP64 archives
- `flatted`: high — flatted vulnerable to unbounded recursion DoS in parse() revive phase, Prototype Pollution via parse() in NodeJS flatted
- `form-data`: high — form-data: CRLF injection in form-data via unescaped multipart field names and filenames
- `glob`: high — glob CLI: Command injection via -c/--cmd executes matches with shell:true, Glob: AbortSignal cancellation bypass allows post-timeout filesystem traversal
- `ip-address`: high — ip-address has XSS in Address6 HTML-emitting methods, ip-address: Address4 decodes leading-zero octets as decimal while resolvers decode them as octal, allowing SSRF and trust-boundary bypass, ip-address: Address6.isLinkLocal() recognizes fe80::/64 rather than fe80::/10, allowing SSRF and trust-boundary bypass to on-link hosts
- `js-yaml`: high — js-yaml has prototype pollution in merge (<<), JS-YAML: Quadratic-complexity DoS in merge key handling via repeated aliases, js-yaml: YAML merge-key chains can force quadratic CPU consumption
- `lodash`: high — lodash vulnerable to Code Injection via `_.template` imports key names, Lodash has Prototype Pollution Vulnerability in `_.unset`, `_.omit`, and `_.pullAt` functions
- `make-fetch-happen`: high — cacache
- `minimatch`: high — minimatch has a ReDoS via repeated wildcards with non-matching literal in pattern, minimatch has a ReDoS via repeated wildcards with non-matching literal in pattern, minimatch has a ReDoS via repeated wildcards with non-matching literal in pattern
- `nanoid`: high — nanoid: non-secure generators can loop indefinitely with negative size, nanoid: custom generators can loop indefinitely when size is zero, nanoid: Integer Overflow or Wraparound
- `picomatch`: high — Picomatch: Method Injection in POSIX Character Classes causes incorrect Glob Matching, Picomatch has a ReDoS vulnerability via extglob quantifiers
- `postcss`: high — PostCSS has XSS via Unescaped </style> in its CSS Stringify Output, PostCSS: Arbitrary file read and information disclosure via attacker-controlled sourceMappingURL in CSS comments, PostCSS: incomplete fix of GHSA-6g55-p6wh-862q — attacker-controlled sourceMappingURL reads arbitrary .map files when `from` is unset
- `protobufjs`: critical — protobuf.js: Code injection through bytes field defaults in generated toObject code, protobuf.js: Denial of service from crafted field names in generated code, protobuf.js: Prototype injection in generated message constructors
- `rollup`: high — Rollup 4 has Arbitrary File Write via Path Traversal
- `source-map-js`: high — source-map-js allows event-loop denial of service through indexed source-map section offsets
- `tar`: critical — node-tar Vulnerable to Arbitrary File Creation/Overwrite via Hardlink Path Traversal, node-tar is Vulnerable to Arbitrary File Overwrite and Symlink Poisoning via Insufficient Path Sanitization, Arbitrary File Read/Write via Hardlink Target Escape Through Symlink Chain in node-tar Extraction

