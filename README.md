# RRAZ filters for Affinity

**Plain page with everything: <https://rraz.github.io/Filters/>**

Standalone filters for Affinity 3 on Windows 10/11 (64-bit). Each filter has its
own installer and is downloaded as one zip. **These filters only work on 16-bit
rasterised images.**

| Filter | What it does | Download | Notes |
|---|---|---|---|
| RRAZ Deblur | Recovers detail from defocus and motion blur. Requires an NVIDIA GPU and driver 580 or newer. | [Deblur 1.0.0](https://github.com/RRaz/Filters-Downloads/releases/tag/deblur-1.0.0) | [Notes (PDF)](https://rraz.github.io/Filters/deblur-notes.pdf) |
| RRAZ Depth | Builds a 16-bit depth map from the selected pixel layer in Affinity. Runs on the CPU, so no graphics card is needed. | [Depth 1.0.0](https://github.com/RRaz/Filters-Downloads/releases/tag/depth-1.0.0) | [Notes (PDF)](https://rraz.github.io/Filters/depth-notes.pdf) |
| RRAZ Save DNG | Saves a 16-bit image as a DNG, so a TIFF can be opened in the Develop persona and developed again later. | [Save DNG 1.0.0](https://github.com/RRaz/Filters-Downloads/releases/tag/savedng-1.0.0) | No installer: two files to copy |

## TIFF and raw files

A TIFF opens as a finished picture. Affinity edits its pixels, so a change is
written into the image, and an earlier state survives only because you saved a
copy under another name.

A raw file is not changed by the Develop persona. The module works on its own
output: the adjustments are kept with the layer, and when you re-enter Develop
the controls are where you left them, ready for another change. The file on disk
stays as it was.

A TIFF has no raw data behind it. Put through the same persona, the adjustments
are applied to the pixels themselves, so re-entering Develop starts again from
the beginning, with every control reset.

That is the point of a non-destructive stack: a change made in Develop shows at
the top of the stack almost at once, and can be revisited and readjusted from the
point you left them. **RRAZ Save DNG
writes the 16-bit image as a raw file**, so a picture that started as a TIFF can
be edited that way. It does not add dynamic range the TIFF never had.

A second use follows from the same thing. At any point the layer as it stands can
be saved as a DNG, so the work so far travels as a raw file: it opens in any
program that reads DNG and can be developed further there. That makes the file a
hand-off to another editor, or a working copy kept in a form that is not tied to
one application.

## Installing a filter

1. Download the zip for the filter. It contains the setup, the runtime, the
   installation sheet and the checksums.
2. Right-click the zip and choose **Extract All**. Choose the folder first: the
   zip and the extracted folder each need as much space as the download.
3. Run the setup from that folder. It does not ask where to install: the engine
   goes to `%LOCALAPPDATA%\RRAZ` on your Windows drive.
5. When it works, delete the zip and the folder you extracted, with everything in
   it.
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
