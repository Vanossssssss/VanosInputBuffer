# Vanos Input Buffer — build package

This package builds a Windows Geometry Dash 2.2081 `.geode` file using GitHub Actions.

**Important:** This is a branded build recipe, not a precompiled `.geode` file. It downloads the open-source implementation from Lyophi's `GMD-Buffer-Mod` repository during the build, changes the mod metadata to Vanos Input Buffer, and builds it with the official Geode build action. The upstream implementation and its MIT license/attribution are retained.

## Build it (no C++ tools needed on your PC)

1. Download and unzip this package.
2. Sign in to GitHub and create a **new repository** (for example `VanosInputBuffer`).
3. Upload the files and folders from this unzipped folder to that repository. Make sure `.github/workflows/build.yml` is included.
4. Open the repository's **Actions** tab. If asked, enable workflows.
5. Open **Build Vanos Input Buffer**, click **Run workflow**, then **Run workflow** again.
6. Wait for the run to finish green. Open that run and download the artifact named **Vanos-Input-Buffer-Windows**.
7. Unzip the artifact. It should contain the `.geode` file. Add that file to your Geode mods folder and launch Geometry Dash.

## Notes

- Target: Windows, Geometry Dash 2.2081.
- Settings are in Geode's mod settings; this does not add a main-menu button.
- The input-buffer behavior comes from the upstream project, not a newly invented implementation.
- If the build fails, open the Actions run and read the error log. The upstream project or Geode SDK may have changed.
