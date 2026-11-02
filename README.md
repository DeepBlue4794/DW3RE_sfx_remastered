# DW3RE Classic Sound Effects

A PC sound replacement mod for **Dynasty Warriors 3: Complete Edition Remastered**, restoring five classic Dynasty Warriors 3 battle notifications: enemy officer defeated, allied officer retreat, information, cheering, and warnings.

The current version, **v0.5**, increases the volume of these replacements. Peak compression can make the sound slightly harsher. The other 48 sounds in the Sys bank remain unchanged. Package and decoding checks pass; v0.5 still needs in-game listening feedback.

## Download and install

1. Download [ClassicAlerts-v0.5.zip](rel/ClassicAlerts-v0.5.zip) (open the file and choose **Download raw file**).
2. Close the game. In Steam, right-click the game and select **Manage > Browse local files**.
3. Remove any previous version of this mod's `.pak`, `.utoc`, and `.ucas` files from `DW3CE_RE/Content/Paks`. Do not remove the original `DW3CE_RE-Windows.*` or `global.*` files.
4. Extract the ZIP and copy its `DW3CE_RE` folder into the game installation folder, merging folders when prompted.
5. Verify that these three files are in `<game installation>/DW3CE_RE/Content/Paks/`:
   - `zDW3_ClassicAlerts_v05_P.pak`
   - `zDW3_ClassicAlerts_v05_P.utoc`
   - `zDW3_ClassicAlerts_v05_P.ucas`
6. Launch the game and test the notification sounds.

Use only one version at a time. Other mods replacing the same Sys sound bank may conflict. No additional mod loader is required.

To uninstall, close the game and remove only the three `zDW3_ClassicAlerts_v05_P` files listed above.

## Repository contents

- `origin_sfx_res/`: original sound files and the source archive's readme.
- `rel/`: the current mod package, installation files, and validation report.
- `doc/`: sound mappings, listening samples, development notes, and [project status](doc/STATUS.md).

## Credits

Thanks to **XthemastaX** for sharing the original sound archive through [Dynasty Warriors 3 Sound Effects and Voices (Download Link in Description)](https://www.youtube.com/watch?v=4xKZqx8m1Hc). The archive's readme identifies PSound201 as the extraction tool. Original game audio belongs to its respective rights holders.
