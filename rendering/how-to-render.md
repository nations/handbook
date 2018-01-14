# How to Render


## Rendering
First, you must have the video assets needed for the render and have downloaded them to the downloads folder for your channel's render PC. Then, locate your channel's render template. For example, on Lil Beast, the Chill Nation template is located in `Desktop/The Nations/Chill Nation/Visualizer/Version 15/`. Within the directory, the AEP files will have this naming schema: `CN_1440p_60_V14.aep`.

1. Once the template has been opened in AE, drag the asset files from Downloads into the Test Files on AE.
2. Go to the first comp, named "Put Wallpaper Here", drag the wallpaper down under Mirror.
3. Go to the second comp, named "Put Track Here", delete the old track if there is any, then drag your track down
4. Go to the third comp, named "Click Apply Here", click on the soundKeysPump layer, then in the effect controls, click on the "Apply" button. Wait a few seconds for it to complete.
5. Go to the fourth comp, named "Click Apply Here Again", click on the soundKeysPush layer, then in the effect controls, click on the "Apply" button. Wait a few seconds for it to complete.
6. Go to the comp named "Render This", then drag the audio file down to the layers. Remember to delete any existing ones first.
7. (For new templates >V14) Select a social to promote by enabling the view of one (twitter/snap/spotify, etc - may vary depending on the Nation). Make sure you only have one selected.
8. Drag the slider to make sure its the same length as the audio file
8. Go to `File` > `Export` > `Add to Render Queue`
10. Click on the render queue, then scroll down to the most recently added render, click on the downwards facing arrow next to "Lossless", then click H.264. Then, click on the file name to the right.
11. Set an output directory, which should be `Desktop/The Nations/Your Nation/Rendered Videos/` - then save the video under the song name.
12. Click the render button, the render should take less than 1h30m usually, depending on the Nation and song length.

## Common Issues

### Render length is not same as song
- You did not drag the slider across correctly, it needs to match the same length as the song layer

### Jittery/uneven logo pulses
- Go to the "Click Apply Here" layer, drag the slider to the length of the song even though you can't visualize it

### Low quality video
- Before rendering, go to the H.264 settings, go to "Format options", up the min bitrate to 6, max to 7
