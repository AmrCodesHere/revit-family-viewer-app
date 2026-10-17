<img src="logo.svg" width="64" height="64" alt="">

# Revit Family Viewer

Open Revit families (`.rfa`) in 3D in your browser, without Revit and without uploading anything.

**Try it:** https://amrcodeshere.github.io/revit-family-viewer-app/
**Or download** `RevitFamilyViewer.html` from [Releases](https://github.com/AmrCodesHere/revit-family-viewer-app/releases/latest).
It is a single file of about 3 MB, opens from disk and works offline.

Drop families or whole folders on the page, or use **Open files** / **Open folder**.

## Your files stay on your computer
Families are read inside the browser tab. Nothing is uploaded, and the page makes no network
requests, whether you open it from the website or from the downloaded file.

## What it shows
- **3D** from the graphics Revit saved in the family, for files saved in **Revit 2024 or later**.
  Coarse, Medium or Fine, as the family shows once placed in a project.
- **Types and parameters**, and a table comparing the types.
- Each card says what you get: **Saved 3D**, **Partial 3D · n%**, **Preview only**, or why a file
  could not be read. "Coverage details" lists every stored face and why any was not drawn.

## Limits
- Files saved **before Revit 2024** show their types, parameters and preview image, but no 3D yet.
- Formulas and constraints are not evaluated. The 3D is the type that was current when the family
  was saved, so choosing another type does not change the model.
- No editing, no type catalogs, no textures (flat material colours), no export.

## Feedback
Found a family that opens wrongly? Please [open an issue](https://github.com/AmrCodesHere/revit-family-viewer-app/issues)
with the Revit version and, if you can share it, the family.

## Licence
Apache-2.0 ([LICENSE](LICENSE)). The viewer includes rvt-rs (Apache-2.0), three.js (MIT) and other
open-source libraries; their licences are in [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt)
and inside the app under *About & licences*.

Not affiliated with or endorsed by Autodesk. Revit is a registered trademark of Autodesk, Inc.
