# MAPPG

MAPPG is a browser-based video mapping tool. Draw polygon shapes, assign animated textures or video, and send the result to a clean output window for projection or display.

## Run

Open `index.html` in a modern browser.

For more consistent browser behavior, you can serve the folder locally:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000/index.html`.

## Use

1. Click points on the canvas to draw a polygon.
2. Double-click, or click near the first point, to close it.
3. Select the polygon and choose a texture.
4. Adjust opacity, speed, blend mode, colors, rotation, tilt, scale, and pan.
5. Click `SAVE SCENE` to download the full scene as a JSON file.
6. Click `LOAD SCENE` to restore a saved JSON scene.
7. Click `LAUNCH OUTPUT` to open the projection window.
8. Double-click the output window to toggle fullscreen.

## Controls

- `D`: Draw tool
- `S`: Select tool
- `X` or `Delete`: Delete selected polygon
- `C`: Curve or straighten the hovered edge
- `Escape`: Cancel drawing or close the color picker

In Select mode, drag a polygon to move it, drag points to reshape it, click an edge to add a point, and Alt-click a point to remove it.

## Video

Select the `Video` texture, then click `+ Load Video File` to use a local video inside the selected polygon.

## Notes

- Keep the editor window open while using the output window.
- Allow popups if the output window does not open.
- `SAVE SCENE` exports polygon geometry, texture choices, colors, visibility, blend, and transform settings.
- `LOAD SCENE` restores saved JSON scene files. Local video files must be loaded again after restoring.
