# RRAZ filters for Affinity

**Plain page with everything: <https://rraz.github.io/Filters/>**

Standalone filters for Affinity 3 on Windows 10/11 (64-bit). Each filter has its
own installer and is downloaded as one zip. **These filters only work on 16-bit
rasterised images.**

| Filter | What it does | Download | Notes |
|---|---|---|---|
| RRAZ Deblur | Recovers detail from defocus and motion blur. Requires an NVIDIA GPU and driver 580 or newer. | [Deblur 1.0.0](https://github.com/RRaz/Filters-Downloads/releases/tag/deblur-1.0.0) | [Notes (PDF)](https://rraz.github.io/Filters/deblur-notes.pdf) |
| RRAZ Depth | Builds a 16-bit depth map from the selected pixel layer in Affinity. Runs on the CPU, so no graphics card is needed. | [Depth 1.0.0](https://github.com/RRaz/Filters-Downloads/releases/tag/depth-1.0.0) | [Notes (PDF)](https://rraz.github.io/Filters/depth-notes.pdf) |

## Installing a filter

1. Download the zip for the filter. It contains the setup, the runtime, the
   installation sheet and the checksums.
2. Right-click the zip and choose **Extract All**. Choose the folder first: the
   extracted files need as much space as the download. Delete the zip once it is
   extracted.
3. Run the setup from that folder. It does not ask where to install: the engine
   goes to `%LOCALAPPDATA%\RRAZ` on your Windows drive.
4. In Affinity, open **Settings > Photoshop Plugins** and add
   `%LOCALAPPDATA%\RRAZ\Affinity`
   (normally `C:\Users\<you>\AppData\Local\RRAZ\Affinity`).

The filter then appears under **Filters > Plugins > RRAZ**. No account, upload
or server is used. The install is per user and does not need administrator
rights. After it works you can delete the extracted folder; the engine stays in
`%LOCALAPPDATA%\RRAZ`.

## Adding the folder to Affinity

The plug-in folder is added once, and the steps are the same for every RRAZ
filter. They are illustrated here:
[Setting up the folder (PDF)](https://rraz.github.io/Filters/setup-affinity.pdf).

If you already have an RRAZ filter working, the folder is already added: close
and reopen Affinity and the new filter is in the menu.

## Notes

The **Notes** link for each filter opens the photographer's notes as a PDF.
They are kept separate from the installer and may be updated at any time.

## Licence and credit

Each filter's installation sheet includes its own algorithm credit and licence.
The photographer's notes have their own licences, stated in the notes folder.
