# Kouseikan browser startup

Original Zzz studio logo animation → Kouseikan loading shell → first rendered game frame. Click or Enter skips the studio intro. Reduced motion and startup failure/retry are supported.

`boot/` contains the loader skin and original project assets. Progress follows each stage reported by the engine. An unknown total uses an indeterminate indicator. The skin preserves the engine's status and first-frame hooks, native input, save import/export and error reporting.

After each Ren'Py web export, run this command **from the source repository CHA-NYANN/NTR** before uploading the generated directory here:

```powershell
python tools/apply_web_boot.py "path/to/web-export"
```

Ren'Py regenerates index.html on export, so this post-export step is required to retain the branding. Source, documentation and contract tests are in NTR's `tools/web_boot/`, `tools/apply_web_boot.py` and `tools/test_web_boot.mjs`.

The default `web-presplash.jpg` is no longer referenced by the page. Its file remains in the export; game.zip, vendor engine, service worker and browser save storage are not modified by the branding tool.
