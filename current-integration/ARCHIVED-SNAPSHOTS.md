# Archived integration snapshots

The 4 files listed below (2,830 physical source lines) were retired from the current tree because they are superseded integration snapshots, not current build inputs.

This product remains paused. Its original Python source and shared module templates remain. The active shared AndroidTools adapter/runtime is owned and built by the remote-notifications submodule, as declared in tool-release.json.

The superproject solution, project includes, tool build scripts, package manifests, and runtime source staging do not consume these paths. Existing Surface XAML, reflection-loaded factory types, shared runtime ownership, original-source trees, and linked tests remain unchanged. No runtime behavior change or build-time speedup is claimed from deleting files that were not compiled.

The later remote SDK/package and named-pipe adjustments to these retired snapshots remain recoverable at the recovery commit below. The remote `.gitignore` is retained unchanged.

## Restore from Git history

Recovery commit in this tool repository: `a8cda6be8d4c499401f2e25f9d9fc1c2e37a61b2`. Keep the repository history containing this commit when publishing or mirroring it. A shallow clone or a source ZIP alone may not contain these historical blobs.

Run from this tool repository after saving any current changes:

```sh
git cat-file -e a8cda6be8d4c499401f2e25f9d9fc1c2e37a61b2^{commit}
git restore --source=a8cda6be8d4c499401f2e25f9d9fc1c2e37a61b2 -- current-integration/src/AndroidTools.MyPowerTools current-integration/src/AndroidTools.Runtime
```

If the commit is absent, obtain it from an existing full clone or the repository remote containing this history before restoring. Restoring adds historical source files to the working tree; it does not wire them back into the current build.

The original source-map capture fields remain historical provenance. Its archivedIntegrationSnapshots entries describe the later retirement and point to this document, which stays inside current-integration so source-bundle materialization preserves it.

## Exact file recovery inventory

| Path | Git blob SHA-1 | Physical lines |
| --- | --- | ---: |
| `current-integration/src/AndroidTools.MyPowerTools/AndroidTools.MyPowerTools.csproj` | `33c0d4bd06845252f9a6c830509ea895020759ae` | 24 |
| `current-integration/src/AndroidTools.MyPowerTools/AndroidToolsModules.cs` | `706b00236159e5035c0aeeb4caf5a8b6ef9ccb3b` | 2239 |
| `current-integration/src/AndroidTools.Runtime/AndroidTools.Runtime.csproj` | `778eb4b24f3aaf7903c7feb2a82f9ff921e50eff` | 32 |
| `current-integration/src/AndroidTools.Runtime/Program.cs` | `c5617ac21a03128b11290834839d88e050e73a45` | 535 |
