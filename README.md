# Mind Palace

Mind maps you lay out by hand. Drag ideas around a canvas, and edit the same map as an outline right next to it: the two always show the same tree.

## Try it

**[Open Mind Palace → petravanta.github.io/mind-palace](https://petravanta.github.io/mind-palace/)**

1. **Start a map.** The picker in the header lists your maps; *+ New map…* starts one from a central idea, or from an outline you paste in (indented lists and Markdown headings both work).
2. **Arrange it on the map.** Drag an idea and its whole branch comes along. Drop it onto another idea to move it under that one. Select an idea and use the toolbar to add a sub-idea or an idea next to it, edit, recolour, fold or delete. Double-tap an idea to edit it.
3. **Edit it as an outline.** On a computer the outline sits beside the map; on a phone, switch with the *Map* and *Outline* tabs. Type to edit, **Enter** adds an idea, **Tab** / **Shift+Tab** move it in or out a level, **Alt+↑/↓** reorder. The buttons above the outline do the same on a phone.
4. **Save it.** Every map stays in your browser. *Settings → Connect Google Drive* syncs all of them through your Drive, and *This map → Save as Google Doc* writes the map as a Google Doc outline.

## What it does

- **One tree, two views.** The canvas and the outline edit the same data, so a change in either shows in the other straight away, and selecting an idea in one selects it in the other.
- **Your layout stays yours.** Ideas stay where you drag them. New ideas go next to their parent, in line with their siblings. *Tidy up* lays the whole map out neatly (main branches split either side of the central idea, in outline order), and undo puts your own layout back. Turn on **Auto-arrange** (the sparkle button by the zoom controls, or *This map*) and the map tidies itself whenever ideas would overlap, as you add, move or type; you can still drag ideas, and where you drop one among its siblings sets its order. The setting is saved with each map.
- **The outline follows the canvas.** After you drag an idea, its siblings are put in canvas order: top to bottom, and main branches clockwise from 12 o'clock. Moving an idea up or down in the outline swaps it with its neighbour on the canvas too.
- **Branch colours.** Each main branch gets its own colour and keeps it when branches are reordered; any idea can pick its own colour, which everything under it shares.
- **Pictures on ideas.** Select an idea and tap the picture button (or tap a thumbnail in the outline) to choose a photo (on a phone: your library or the camera), search free pictures from Wikimedia Commons by keyword, or use a link. You can also drop a picture onto any idea, from your computer or another web page, or paste one with an idea selected. *Search Google Images* opens the same words in Google Images in a new tab to drag or copy a picture from. Pictures are shrunk to 240 px before they're saved, so they sync with the map and go into the Google Doc.
- **Costs.** Give any idea a cost with the coin button, or turn on *This map → Show costs* to get a cost box on every outline row (Enter moves down the column, like a spreadsheet). Every idea with costs under it shows **Σ** and the total of its whole branch, its own cost included, on the map and in the outline; totals follow every edit, move and delete. Each map has its own currency or unit ($, €, Ft, hours…). Costs go into the Google Doc and Markdown exports.
- **Fold** a branch to hide what's under it (in both views); the map shows how many ideas are hidden.
- **Undo and redo** for every change (Ctrl+Z / Ctrl+Shift+Z or the toolbar).
- **Phone first.** Touch drag, pinch to zoom, drag the background to pan, a toolbar within thumb reach. Installs as an app (Chrome: *Install app*; iPhone: *Share → Add to Home Screen*) and opens offline.
- Light and dark themes, the shared **All apps** menu and theme switch, as the [shared standards](https://github.com/petravanta/general/blob/main/STANDARDS.md) describe.

Keys on the map: **Tab** adds a sub-idea, **Enter** an idea next to this one, **F2**, **Space** or just typing edits, the arrows move between ideas, **Delete** deletes, **+** / **−** zoom.

## Saving and exporting

- **Save as Google Doc** (*This map*): the map becomes a Google Doc in your Drive, with the central idea as the title and every idea as a nested bullet. Saving the same map again updates that doc.
- **Download Markdown** / **Copy outline** (*This map*): the same outline as Markdown.
- **Export backup** / **Import…** (*Settings*): every map as one JSON file, merged back in on import. Import also takes a Markdown or text outline as a new map.

## Your data

Nothing is uploaded to a server of ours. Maps live in your browser (`localStorage`). **Settings → Connect Google Drive** keeps a copy of all of them in `Mind Palace data.json` in your own Drive and merges it with the browser copy on connect and whenever the app comes back into view. It uses the `drive.file` permission, so the app only sees files it created (that file and the Google Docs it saved). This follows the *User data* section of the shared standards; Drive uses the shared OAuth client for `https://petravanta.github.io` (`GOOGLE_CLIENT_ID` in the script).

## Publishing

GitHub Pages serves this repo from the `main` branch, root folder (Settings → Pages → Deploy from a branch → `main` / `/ (root)`). The `.nojekyll` file makes Pages serve files as they are.
