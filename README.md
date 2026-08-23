# Multitake — runtime assets

The Core ML separation models [Multitake](https://multitake.studio/) fetches the first time
someone separates a song. Nothing here is source: the models are Meta's Demucs, released under
the MIT licence, converted and compiled by `Tools/export_core.py` and `Tools/upload_models.sh`
in the app's own repository.

They live here rather than in the app because a hundred megabytes in the binary is paid by every
download on every platform, and because a model can then be replaced without an App Store
release.

Releases:

- `models-v1` — `demucs-4-parts.aar`, `demucs-6-parts.aar`. AppleArchive of the compiled
  `.mlmodelc`, expanded by the app into its `Documents/Models` folder.
