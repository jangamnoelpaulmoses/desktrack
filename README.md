# DeskTrack

**Know what you actually did today — without connecting a single app.**

Routine and productivity trackers make you wire up Slack, Notion, email, and calendar APIs before they're useful. DeskTrack takes a different approach: it periodically *looks at your screen* the way you do, uses AI to understand what you're working on, and turns that into your day — automatically, for every app you use, even ones with no API at all.

## What you get

- **Timeline of your day** — what you did, when, in which app, merged into clean sessions
- **Focus score & category breakdown** — where your time really went
- **Auto-detected tasks** — todos, deadlines, and unanswered messages spotted on your screen, prioritized
- **Distraction nudges** — a gentle notification when you've drifted for 10+ minutes (menu bar and floating pill turn amber first)
- **Today's focus** — write down your intention; DeskTrack nudges you when your activity stops matching it
- **Day in review** — an AI-written evening summary: what got done, where time leaked, what to try tomorrow
- **Instant manual capture** — ⌘⇧D from anywhere, or the floating on-screen button

## Privacy, up front

- **Everything stays on your Mac.** Activity log, tasks, summaries — all local files.
- **Screenshots are analyzed and immediately discarded — never stored.**
- Password managers and windows with sensitive titles (banking, incognito, medical…) are **never captured**.
- One-click **Delete all data**. Pause any time from the menu bar.
- Choose your AI: your own OpenAI key, a **fully local model** (via [Ollama](https://ollama.com) — nothing ever leaves your Mac), or **no AI at all** (app-name tracking only, zero setup).

## Download & install

Grab the right file from the **[Releases page](../../releases/latest)**:

| Your Mac | File |
|---|---|
| Apple Silicon (M1/M2/M3/M4) | `DeskTrack-x.x.x-arm64.dmg` |
| Intel | `DeskTrack-x.x.x.dmg` |

(Not sure? Apple menu →  About This Mac — "Chip: Apple M…" means Apple Silicon.)

1. Open the DMG and drag **DeskTrack** into **Applications**.
2. **First launch:** macOS will block it ("Apple could not verify…") because this build isn't notarized yet. One-time fix:
   - **macOS 15 Sequoia+**: open it once, then System Settings → Privacy & Security → scroll down → **Open Anyway**.
   - **macOS 14 and earlier**: right-click the app → Open → Open.
3. **Pick your AI** in the setup panel: paste an OpenAI API key (tested live before saving), click *Use local AI* if you run Ollama, or *Disable AI* for key-free basic tracking.
4. **Grant Screen Recording** when prompted (System Settings → Privacy & Security → Screen Recording → enable DeskTrack), then restart the app.

> **Permission loop?** If macOS keeps saying DeskTrack can't see the screen even though the toggle is ON: click **Deny** on the prompt, quit DeskTrack, reopen it, enable the *fresh* DeskTrack row that appears, and restart. The app also detects this situation and walks you through it.

## Cost

With your own OpenAI key, DeskTrack analyzes the screen only when it meaningfully changes — typically **a few cents per day**. Local and AI-off modes are free.

## Requirements

macOS 13+ recommended (works on 10.15+). Apple Silicon or Intel. For local AI: Apple Silicon with 8 GB+ RAM and Ollama with a vision model (`ollama pull qwen2.5vl:3b`).

## Feedback

Found a bug or have an idea? [Open an issue](../../issues) — this is an early build and feedback shapes what gets built next.
