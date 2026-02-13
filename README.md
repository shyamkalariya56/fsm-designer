# FSM Designer

A professional **Hierarchical Finite State Machine (HFSM) diagram tool** that runs entirely in a single HTML file — no install, no server, no dependencies, no account required.

Open the file in any browser and start designing.

![FSM Designer Screenshot](screenshot.png)

---

## Live Demo

👉 **[Try it live](https://yourusername.github.io/fsm-designer)**

---

## What is it?

FSM Designer lets you visually design and document finite state machines and hierarchical state machines (nested FSMs). It is aimed at **embedded systems engineers, robotics developers, automation programmers, and PLC developers** who need to design and document state logic before or during implementation.

---

## Features

**Diagram**
- 4 state types — `INIT`, `IDLE`, `NORMAL`, `FAULT` — each with distinct colour coding
- State cards show: name, brief description, entry action, exit action, timeout
- Transition arrows with event label and action
- Self-loop transitions
- Bi-directional transitions rendered with offset to avoid overlap

**Hierarchical FSM**
- Any state can contain a nested sub-FSM (up to 3 levels deep)
- Drill in / navigate out via breadcrumb
- Project tree sidebar shows full machine hierarchy

**State Properties**
- Name, number, type
- Brief description (shown on card)
- Entry action — runs when entering the state
- Exit action — runs when leaving the state
- Timeout (ms)
- Sub-FSM toggle

**Transition Properties**
- Event / condition label
- Action — runs on the transition
- Notes / guard condition

**Canvas**
- Drag states freely
- Zoom with `Ctrl + scroll` (15% → 300%)
- Pan with `Space + drag` or scroll
- FIT button auto-fits all states in view
- Connect tool or drag from port `+` to wire states

**Export**
- `PNG` — raster image at 2× resolution
- `SVG` — vector file (lossless, opens in Illustrator / Inkscape)
- `PDF` — print-ready, auto-scaled to A4 landscape

**Save / Load**
- Save as `.json` — full project including all sub-machines
- Load `.json` — restores complete diagram

---

## How to Use

**Option 1 — Download and open locally**
1. Download `index.html`
2. Double-click it — opens in your browser
3. Done. No install needed.

**Option 2 — Use the live demo**
Go to the link above. Everything runs in your browser, nothing is sent to a server.

---

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Double-click` canvas | Add new state |
| `Double-click` state | Edit properties |
| `Del` / `Backspace` | Delete selected state or transition |
| `Ctrl + Scroll` | Zoom in / out |
| `Space + Drag` | Pan canvas |
| `Escape` | Cancel current connection |

---

## State Types

| Type | Colour | Typical Use |
|------|--------|-------------|
| `INIT` | Green | Power-on, initialisation, startup sequence |
| `IDLE` | Purple | Waiting for command, standby |
| `NORMAL` | Cyan | Active operational states |
| `FAULT` | Red | Error states, e-stop, fault handling |

---

## File Structure

```
index.html    ← entire application, single file, ~1100 lines
README.md     ← this file
screenshot.png
```

No build step. No `node_modules`. No framework. Just HTML, CSS, and vanilla JavaScript.

---

## Why single file?

- Works offline — useful on factory floors, embedded lab environments, air-gapped systems
- Easy to share — send one file over email or Slack
- Easy to version — one file in git
- No dependencies to maintain or update

---

## Contributing

Contributions welcome. Open an issue or submit a pull request.

If you find a bug or want a feature, open an issue and describe it clearly.

---

## License

MIT — free to use, modify, and distribute.

---

*Built for engineers who need to think in states.*
