# Jet Lag DC 2026 — Challenge Cards

A single-page web app that deals random challenge cards from a shuffled deck. Built for Jet Lag DC 2026.

## How It Works

1. On load, the app fetches `cards.csv` (one challenge per line) and shuffles all 50 cards.
2. Four cards are dealt into a 2×2 grid.
3. Click **Done ✓** on a card to dismiss it — a new card is drawn from the deck and fades in.
4. When the deck runs out, empty slots show "No more cards!"
5. Click **Reset / New Round** to reshuffle and start over.

## Running Locally

Serve the directory with any static file server:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000).

## Files

| File | Description |
|------|-------------|
| `index.html` | App (HTML + CSS + JS, no dependencies) |
| `cards.csv` | Challenge cards, one per line |

## Customizing Cards

Edit `cards.csv` — one challenge per line, plain text, no header. The app adapts to any number of cards.
