# Changelog

## [Unreleased]

- Replace the copyright placeholder.
- Complete browser, offline-network, accessibility, GPU, morphology, quality-switching, and stability tests.

## [1.0.0] - YYYY-MM-DD

### Added

- Initial public release based on version 51.
- Fully inlined offline `index.html`.
- GPU scalar field, visual fallback, riverbed morphology, uncertainty view, and public compliance documents.

### Refactored

- Extracted `alongFlow` and `flowCrossDistance` for repeated vector calculations.
- Extracted `fluidAtlasSize` for grid-tier atlas dimensions.
- Replaced repeated initialization literals with `FLUID_ABSORB`, `FLUID_MAX_REF_INIT`, `DEFAULT_PARAMS`, and `FLUID_GRID_TIERS.standard`.
- Removed blank lines without intentionally changing model equations, shader equations, UI behavior, dependencies, privacy behavior, or network behavior.

### Security and privacy

- No application-managed persistent storage.
- No application-owned network request or analytics feature.
