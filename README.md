# 3D Scalar Field Sandbox

3D Scalar Field Sandbox is a self-contained educational web application for exploring a hypothetical relative scalar field, simplified time-response behavior, uncertainty, and an illustrative GPU-driven riverbed morphology visualization.

Repository-root `index.html` is the offline release. React, ReactDOM, D3, Three.js, OrbitControls, and generated Tailwind CSS are bundled into the file.

## Demo

Try it here!

https://analyst-mm-2749261.github.io/riverbed-fluid-3d-simulator/

## Features

- Simplified completely mixed relative-value model.
- WebGL2 GPU scalar-field renderer with MacCormack advection and volume ray-marching.
- Illustrative riverbed erosion, mobile-sediment, deposition, and avalanche behavior.
- Independent erosion and deposition controls and five riverbed display modes.
- Voxel-based fallback when required WebGL2 capabilities are unavailable.
- Interactive inlet, outlet, source, and simulated sensor positions.
- Synthetic-data uncertainty view.
- Mobile-oriented playback, presets, parameter sheets, and touch controls.
- No application-managed persistent browser settings.
- Shared flow-geometry and fluid-atlas calculations refactored in version 51.

## Scope and limitations

All displayed values are relative, approximate, hypothetical, or visualization-derived. This is not a validated CFD solver, sediment-transport model, river-engineering model, erosion or deposition predictor, geotechnical tool, physical measurement system, safety system, or basis for operational, engineering, environmental, medical, or regulatory decisions.

The field-sample value is read from the internal simulated dye field, not physical sensor hardware. Riverbed relief in `cm` is a visualization-derived scale, not a surveyed, measured, calibrated, or site-specific elevation change.

See [MODEL_SCOPE.md](MODEL_SCOPE.md) and [DISCLAIMER.md](DISCLAIMER.md).

## Privacy

The offline release contains no analytics, advertising, account, upload, remote API, or application-data transmission feature. State exists only while the page is open. The interface may optionally request device-orientation access and may use a short vibration for touch feedback.

See [PRIVACY.md](PRIVACY.md).

## Running

Download the complete repository or release archive and open `index.html` in a current browser. WebGL2 is recommended. Performance depends on browser, GPU, driver, device temperature, and quality setting.

## Development source

Readable JSX source is stored at `source/3d-scalar-field-sandbox-v51.cdn-source.html`. It deliberately loads dependencies from CDNs and uses runtime Babel; it is not the offline release.

## Redistribution

When redistributing `index.html`, also distribute `THIRD_PARTY_NOTICES.md` and the complete `third_party/licenses/` directory.

## Contributions and security

This repository may be operated as a read-only educational reference with Issues and pull requests disabled. See [CONTRIBUTING.md](CONTRIBUTING.md) and [SECURITY.md](SECURITY.md).

## License

Original project code is licensed under the MIT License after the copyright placeholder in [LICENSE](LICENSE) is replaced. Bundled third-party software remains subject to its own licenses.
