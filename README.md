# RRAZ filters for Affinity

Standalone filters for Affinity 3 on Windows 10/11 (64-bit). Each filter has its
own installer. **These filters only work on 16-bit rasterised images.**

| Filter | What it does | Install | Notes & images |
|---|---|---|---|
| RRAZ Deblur | Recovers detail from defocus and motion blur. Requires an NVIDIA GPU and driver 580 or newer. | [Install & check](https://github.com/RRaz/Filters/releases/tag/deblur-1.0.0) | [Open](https://github.com/RRaz/Filters/tree/HEAD/Deblur/) |
| RRAZ Depth | Builds a 16-bit greyscale depth map from the active layer. Runs on the CPU, so no graphics card is needed. | [Install & check](https://github.com/RRaz/Filters/releases/tag/depth-1.0.0) | [Open](https://github.com/RRaz/Filters/tree/HEAD/Depth/) |

## Installing a filter

1. Open **Install & check** and download the setup, the runtime and the
   installation sheet.
2. Keep the setup and runtime in the same folder. Run the setup.
3. In Affinity, open **Settings > Photoshop Plugins** and add
   `%LOCALAPPDATA%\RRAZ\Affinity`
   (normally `C:\Users\<you>\AppData\Local\RRAZ\Affinity`).

The filter then appears under **Filters > Plugins > RRAZ**. No account, upload
or server is used. The install is per user and does not need administrator
rights.

## Adding the folder to Affinity

The plug-in folder is added once, and the steps are the same for every RRAZ
filter. They are illustrated here:
[Setup filters affinity (PDF)](Setup%20filters%20affinity.pdf).

If you already have an RRAZ filter working, the folder is already added: close
and reopen Affinity and the new filter is in the menu.

## Notes and images

The **Notes & images** link for each filter opens a folder with the
photographer’s notes and example images. They are kept separate from the
installer and may be updated at any time.

## Licence and credit

Each filter’s installation sheet includes its own algorithm credit and licence.
The photographer’s notes and example images have their own licences, stated in
the filter folder.
