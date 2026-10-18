# Process Monitor

This repository preserves the complete Process Monitor source while the product
is paused in the current MyPowerTools delivery plan.

- `original-source/powertool/page2.py` is the original UI entry.
- `current-integration/` retains the shared module templates and archive recovery record.
- `tool-release.json` declares the paused state and package owner.

The active shared adapter package is currently built by the
`remote-notifications` submodule. A future reactivation must first split the
shared `AndroidTools.MyPowerTools` assembly into an independent package.

## Historical integration snapshots

The superseded duplicate AndroidTools adapter/runtime snapshots now live in Git history rather than the current source tree.
See [the exact file inventory and recovery commands](current-integration/ARCHIVED-SNAPSHOTS.md).
Original product source and active build/package inputs remain in place.
