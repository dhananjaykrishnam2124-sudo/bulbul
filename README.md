# Anu's birthday site
Passcode gate -> hold & release -> reveal -> balloons (reasons) -> chocolate cake -> photos -> letter -> finale -> Perfect player.

## Run locally (must be served, NOT opened by double-click, or audio is silent)
    python3 -m http.server 8000   # then open http://localhost:8000

## Deploy (GitHub Pages)
1. Create a repo, upload everything in this folder (index.html, assets/, .nojekyll).
2. Settings -> Pages -> Deploy from branch -> main / root.
3. Open https://<user>.github.io/<repo>/ on the phone.

## Lyrics sync
1. Open the site with ?sync (e.g. https://you.github.io/repo/?sync) and enter the passcode.
2. Paste the lyrics (one line per row) into the box and press Start. The song plays.
3. Tap the button exactly as each line starts. At the end a box shows the timed file.
4. Copy it into assets/lyrics/perfect.lrc, commit, and the lyrics view will highlight in sync.
Format: [01:23.45]line text. Edit any timestamp by hand to fine-tune.

## Change things
Passcode: change PIN_HASH in index.html (sha256 of "anu-" + code). Reasons / letter: REASONS and LETTER at the top of the script.
