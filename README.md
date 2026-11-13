# santoshkanumuri.qzz.io, rebuilt

A one-page portfolio for Santosh Kanumuri. It's a single `index.html` with no build step, no framework and no trackers.

## The idea

The page centres on one timeline that runs from about 1455 to today. Grey marks above the line are moments when machines took on more of our reading, counting, finding or answering: Braille, Snow's cholera map, Hollerith's census, ELIZA, the relational model, PDF, WCAG, RAG, MCP. Orange marks below the line are Santosh's own work.

The scale is linear and honest, so at full width his work is one tight orange stack at the far right. **Zoom in to my work** pulls the stack apart. The line has three views (the last 571, 75 and 10 years), and stepping through with **Later →** moves between them on its own.

- Marks that would overlap stack away from the line instead, so every one stays visible and clickable.
- Names appear as small flags wherever there is room. Hover or focus any other mark to see its name.
- Each work entry links back to the moments it descends from. Each moment links forward to the work that continues it.

The rest of the page:

- **Work**: eight systems, each with *How it works* (the pipeline), *Tested against* (the real-world numbers), *Lineage* and *Built with*.
- **Built to find out**: side projects listed as the questions that started them.
- **Errata**: a standing offer to correct any wrong date or number, with credit.

## Accessibility

- Body type is Atkinson Hyperlegible Next and Mono, commissioned by the Braille Institute for low-vision readers.
- Every colour passes WCAG AA contrast in both light ("Morning") and dark ("Evening") themes, switched from the header.
- The timeline uses a roving tabindex. Use ← → / Home / End to move between moments, and changes are announced through a polite live region. The full timeline is also available as a plain list with sources.
- `prefers-reduced-motion` turns off the zoom animation and every transition.

## Run it

Open `index.html` in a browser. To host it on GitHub Pages: **Settings → Pages → Deploy from a branch**, then choose the root folder.

## Editing

- Timeline moments live in the `EVENTS` array near the bottom of `index.html`. `y` is a fractional year, `name` is the short flag text, and every world event has a `src` link.
- Work entries are the `<li id="w-…">` blocks. Side projects are the `<li id="q-…">` blocks.
- Colours and type are the tokens at the top of the `<style>` block.
