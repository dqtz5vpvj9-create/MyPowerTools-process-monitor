# Process Monitor

This repository preserves the complete Process Monitor source while the product
is paused in the current MyPowerTools delivery plan.

- `original-source/powertool/page2.py` is the original UI entry.
- `current-integration/` records the current shared AndroidTools adapter state.
- `tool-release.json` declares the paused state and package owner.

The active shared adapter package is currently built by the
`remote-notifications` submodule. A future reactivation must first split the
shared `AndroidTools.MyPowerTools` assembly into an independent package.
