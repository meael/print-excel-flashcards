# print-excel-flashcards

Printable flashcards from Excel vocabulary files. A single-page web app with no build step and no backend — runs entirely in the browser.

**Open:** https://meael.github.io/print-excel-flashcards/

## What it does

- Load one or more `.xls` / `.xlsx` files
- Pick the "Front" (word) and "Back" (translation) columns — columns are auto-detected
- Lays out business-card–sized flashcards (85×54 mm), 10 per A4 sheet
- Prints double-sided cards by hand (no auto-duplex): fronts first, then backs with a mirrored layout for flipping on the long or short edge
- Options: cut lines, "first sheet only" test mode

## How to print

1. Enable "test", click **Print fronts**. In the print dialog: scale **100%**, margins **none**.
2. Flip the sheet on the long edge, put it back in the tray.
3. Click **Print backs**, check alignment against the light.
4. If left–right is swapped, switch "Flip" to short edge and repeat the test.
5. Disable "test" and print everything: fronts first, then backs.

## Stack

Plain HTML/CSS/JS. Excel parsing via [SheetJS](https://sheetjs.com/) over CDN. Data never leaves the browser.

## Run locally

Open `index.html` in a browser. No server needed.
