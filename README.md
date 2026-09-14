# KOsT

A minimalist expense tally. Add an item and its price, watch the running total update, and export the list as a CSV or print it as a PDF when you're done. Built for quick, no-friction tracking rather than full budgeting — no accounts, no categories, no setup. Supports light and dark themes.

## Features

- **Add and total** — type an item and a price, hit enter or the `+` button, watch the total update
- **Quantity** — an optional Qty field lets you note things like `2` or `2kg` alongside the item name (e.g. "2 Coffee", "2kg Sugar"); price is still entered as the total for that line
- **Edit in place** — click any item's name, quantity, or price to correct it without deleting and re-adding (quantity can only be edited after it's set on add — there's no way to add a quantity to an existing item later)
- **Day grouping** — entries are stamped with the date they were added and grouped once you're tracking across more than one day, each with its own subtotal
- **Persistence** — your list and theme choice are saved locally in the browser and survive a refresh
- **Light / dark theme** — toggle in the top corner; your choice is remembered
- **Export** — download a CSV of the full list, or print/export as PDF
- **No accounts, no backend** — everything runs client-side in a single HTML file

## Usage

Just open `KosT.html` in a browser. There's no build step and no server required.

```bash
open KosT.html   # macOS
# or double-click the file, or serve it locally:
python3 -m http.server
```

## Notes

- Data is stored in `localStorage`, scoped to the browser and device you're using — it won't sync across devices, and clearing browser data will clear your tally.
- Currency is displayed in ₹ (INR) by default.
- "Clear all" is permanent and asks for confirmation before wiping your list.

## License

MIT
