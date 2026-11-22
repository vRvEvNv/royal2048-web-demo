# ROYAL 2048 — Browser Demo

A physics-based number-merging puzzle game with jelly pieces and eight game modes.
This demo has no advertising or in-app purchases.

The landscape interface keeps the original portrait board in the center. Mode,
score and countdown appear on the left; Home, Music and Sound remain on the
right. The home screen centers a cropped castle garden behind the logo and stacked
New Game / Back to Game buttons. The eight-mode selection grid adapts to wide screens.
Narrow screens use a compact portrait layout. Best Records and Privacy links
have been removed; current-round scores and unfinished-game saves remain.

## GitHub Pages

Publish the contents of this folder at the root of your repository. Keep all
`index.*` filenames unchanged and include `.nojekyll`. In Settings → Pages,
select **Deploy from a branch**, **main**, and **/ (root)**.

Use GitHub Desktop or Git to upload: the game pack and WebAssembly module exceed
the GitHub browser uploader's 25 MiB per-file limit. Do not upload the ZIP itself
as the website, and do not put `index.html` inside another folder.

## Local preview

Serve this folder over HTTP, for example with `python3 -m http.server 8060
--bind 127.0.0.1`, then open http://127.0.0.1:8060/ in your browser. Do not open
`index.html` directly as a file. Click/tap in the game to enable audio if needed.
After replacing an older build, force-refresh the browser (Command+Shift+R on
Mac) to load the updated game and page layout.

Built with Godot 4.5.2, Compatibility renderer, single-threaded Web export.
The demo requires a browser with WebAssembly and WebGL 2 support. It does not
require cross-origin isolation headers. This is an initial demo for evaluation;
Poki SDK integration has not been added.

The Godot Engine license is in `GODOT_LICENSE.txt`. Font license texts are
included in the game pack. The engine license does not license the game's
artwork or other original content.

This optimized build reduces the game pack to about 5.3 MB. In-game image
resolutions are retained; unused artwork is excluded and large textures use
high-quality compression. Home music uses a smaller stereo Vorbis stream;
full track lengths, looping and lossless short sound effects are retained.
