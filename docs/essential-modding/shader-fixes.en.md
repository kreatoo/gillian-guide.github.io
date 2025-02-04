title: Shader Fixes
description: One of the must-have mods for your GTA IV install

# Shader Fixes
!!! warning "Compatibility" 
    This mod is compatible with the Complete Edition, as well as patches 1.0.7.0 and 1.0.8.0.

This project aims to fix and restore broken and missing shaders on the PC port (everything from [here](https://libertycity-ru.translate.goog/gta-4/articles/4346-gta-iv-complete-edition-xbox-protiv-pc.html?_x_tr_sl=ru&_x_tr_tl=en&_x_tr_hl=pt-BR)). You can read the changelog [here](https://github.com/Parallellines0451/GTAIV.ShaderFixesCollection/blob/main/README.md#feature-list).

## Installation { data-search-exclude }
You can either install this mod as a standalone, as a part of [IV Tweaker](../../extras/modloading/#iv-tweaker), a part of [UAL's modloader](../../extras/modloading/#ultimate-asi-loader) or update the files in [FusionFix](fusionfix.md) which already contains this mod.

=== "Standalone"
    * Go to the [Releases](https://github.com/Parallellines0451/GTAIV.ShaderFixesCollection/releases) page.
    * Download the latest version.
    * Extract the files from the :material-folder:==1. Main== into the game folder, replacing all files when prompted.
    ???+ tip "Console-like Gamma"
        If you also want to have console-like gamma, extract :material-folder:==2. Addons\Console-like Gamma== into the game folder, replacing all files when prompted.
        <figure markdown>
            ![Console gamma](assets/console-gamma.png)
            <figcaption></figcaption>
        </figure>


=== "Part of UAL's modloader | Updating FusionFix files"
    * Go to the [Releases](https://github.com/Parallellines0451/GTAIV.ShaderFixesCollection/releases) page.
    * Download the latest version.
    * Extract the files from the :material-folder:==1. Main== to the :material-folder:==update==, replacing all files if prompted.
    ??? tip "Console-like Gamma"
        If you also want to have console-like gamma and ==you're not using FusionFix==, extract :material-folder:==2. Addons\Console-like Gamma== to :material-folder:==update==, replacing all files when prompted.
    <figure markdown>
        ![Console Gamma](assets/console-gamma.png)
        <figcaption></figcaption>
    </figure>

=== "Part of IV Tweaker"
    !!! warning ""
        This is not recommended due to potential incompatibility issues. Use the UAL's modloader method or [latest FusionFix port](fusionfix.md) instead.
    * Go to the [Releases](https://github.com/Parallellines0451/GTAIV.ShaderFixesCollection/releases) page.
    * Download the latest version.
    * Create a mod folder in :material-folder:==modloader==.
    * Extract the files from the :material-folder:==1. Main\common\shaders\win32-30== (or any other folder in there) into the mod folder.
    !!! info ""
        Alternatively you can grab the mod folder from [here](https://zolika1351.pages.dev/mods/ivtweaker/downgrading) in optional mods and just extract that.
    * Configure :material-file-cog:`modloader.ini` if needed.

[:material-page-first:Previous page <br>ZolikaPatch</br>](fusionfix.md){ .md-button } [Next page:material-page-last: <br>Multiplayer</br>](../multiplayer.md){ .md-button .md-button--primary }