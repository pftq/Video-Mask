# Video-Mask
Tool to quickly draw masks on videos without loading up Adobe Premiere or After Effects.

Download here: https://github.com/pftq/Video-Mask/releases/tag/20261121<br>
You may also find these useful (one-click to download all [here](https://drive.google.com/drive/folders/1nvQFC5uwsZlf-82LuskCP-qut9xHw-lt?usp=sharing)):\
• [Video Debanding](https://github.com/pftq/Video-Debanding) (fixes quality issues with repeat re-processing/compression)\
• [Video Compare](https://github.com/pftq/Video-Compare) (to check export errors, differences, etc)\
• [MP4 Audio Delay Fix](https://github.com/pftq/MP4-Audio-Delay-Fix) (20ms delay at start of file)\
• [Video Frame Sync](https://github.com/pftq/Video-Frame-Sync) (syncing 2 files that drift out of sync)\
• [Video Color Match](https://github.com/pftq/VideoColorMatch) (correcting color grading drift)\
• [Video Splicer](https://github.com/pftq/Video-Splicer) (trim or join MP4s without re-encoding)\
• [Screencaps Generator](https://github.com/pftq/Screencaps-Generator) (smart screencaps selection + gallery grid sheet)\
• [Video To Selective Color](https://github.com/pftq/Video-To-Selective-Color) (selectively leave things in color on black-and-white video)

Made mainly to complement the VideoFrameSync and VideoColorMatch tools I also have that can work with masks (such as for the WAN VACE Masking workflow I created [here](https://civitai.com/models/1536883/wan-vace-masking-and-extension-seamlessly-extend-join-and-auto-fill-existing-videos-while-maintaining-motion)).  I used to use Adobe Premiere and After Effects to manually draw masks, but it's so heavy and slow.  This tool loads up in seconds and is very fast, doesn't lag.

It also now includes the functionality of VideoFrameSync and VideoColorMatch so you can sync, color-correct, and merge the changes back to the original clip in the same tool.

<img width="1074" height="747" alt="image" src="https://github.com/user-attachments/assets/f2d19a54-c994-4f37-8266-419ffd1e205b" />

<img width="1071" height="740" alt="image" src="https://github.com/user-attachments/assets/94158590-ed46-4b58-ba5c-3358809c9c0d" />

You then take the masked video and feed it into WAN VACE to "auto-fill" the masked areas.

Examples:

https://github.com/user-attachments/assets/c3091aa4-dd06-46d9-b489-248c340f6bd3

https://youtu.be/0gx6bbVnM3M

https://youtu.be/_fmc-Ovh5CU


Timelapses of what it's like editing with this process:

https://youtu.be/4iGRRb6P10U

https://www.youtube.com/watch?v=oK_g9JxLPvw

Credits:

Python, application runtime

Tcl/Tk, desktop interface and interactive mask editor

NumPy, frame and mask calculations

OpenCV, mask expansion, shrinking, and feathering

Pillow, frame previews and mask overlays
PyAV / FFmpeg, video and audio decoding, encoding, and MP4 export
PyInstaller, Windows executable packaging
