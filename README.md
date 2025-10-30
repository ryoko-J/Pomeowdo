# 🐾 Pomeowdo v1

> “Focus.exe is now running.”
> — Mochi, probably

**Pomeowdo** is a pixel-cat Pomodoro timer for people who take their naps as seriously as their grind.
It’s cozy chaos in a single HTML file — a self-aware parody of hustle culture where cats manage your focus cycles and roast your life choices.

Each cat embodies a different archetype of existence —
the stoic, the caffeinated, the nihilist, the gremlin — all looping between focus and futility with adorable efficiency.

---

## 🌙 Features

- 🕒 Pomodoro / Short / Long modes
- 💤 Sleep / Wake toggle with animated fade transitions
- 🐈‍⬛ 7 unique cats, each with their own personality and quotes
- 💬 Distinct wake-up and idle quote pools per cat
- 💾 Auto-save of cat, mode, and timer state (via localStorage)
- 💬 Rotating “affirmations” of questionable wisdom
- 🔊 Full emotional sound engine (MEOW, MRRP, TRILL, PURR, SHORT, LONG)
- ⚡ 100 % offline, lightweight, and zero dependencies
- 🌐 Deployable to **Vercel** in under 30 seconds

---

## 🧩 Sound Logic Map

| Event                  | Sound         | Description                  |
| ---------------------- | ------------- | ---------------------------- |
| Start (awake)          | **MEOW.mp3**  | happy start cue              |
| Start (while sleeping) | **TRILL.mp3** | annoyed wake-up (skips MEOW) |
| Manual Sleep → Sleep   | **PURR.mp3**  | entering sleep               |
| Manual Sleep → Wake    | **MRRP.mp3**  | gentle normal wake           |
| Change Cat             | **MEOW2.mp3** | playful chirp                |
| Pomodoro End           | **LONG.mp3**  | long chime                   |
| Short Break End        | **SHORT.mp3** | short chime                  |

All `.mp3` files live in `/assets/sfx/`.

---

## 🗂 Folder Structure

```
project/
├── index.html
├── vercel.json
├── credits.json
├── README.md
└── assets/
    ├── sfx/
    │   ├── MEOW.mp3
    │   ├── MEOW2.mp3
    │   ├── MRRP.mp3
    │   ├── TRILL.mp3
    │   ├── PURR.mp3
    │   ├── SHORT.mp3
    │   └── LONG.mp3
    └── cats/
        ├── mochi_idle.gif
        ├── mochi_run.gif
        ├── mochi_sleep.gif
        ├── ash_idle.gif
        ├── ash_run.gif
        ├── ash_sleep.gif
        ├── chai_idle.gif
        ├── chai_run.gif
        ├── chai_sleep.gif
        ├── sumi_idle.gif
        ├── sumi_run.gif
        ├── sumi_sleep.gif
        ├── nyx_idle.gif
        ├── nyx_run.gif
        ├── nyx_sleep.gif
        ├── bean_idle.gif
        ├── bean_run.gif
        ├── bean_sleep.gif
        ├── tora_idle.gif
        ├── tora_run.gif
        └── tora_sleep.gif
```

---

## ⚙️ Deployment (Vercel)

1. Clone or fork this repo.
2. Push it to GitHub.
3. Deploy via [Vercel](https://vercel.com) → “New Project.”
4. Ensure `vercel.json` includes:

```json
{
  "builds": [{ "src": "index.html", "use": "@vercel/static" }],
  "routes": [{ "src": "/(.*)", "dest": "/index.html" }]
}
```

5. Done. Bask in the glory of **Pomeowdo** — where productivity and absurdism hold paws.

---

## 🧠 Cat Pantheon

| Cat       | Archetype              | Motto                                            |
| --------- | ---------------------- | ------------------------------------------------ |
| **Mochi** | Gentle Procrastinator  | “Be honest… did you hydrate?”                    |
| **Ash**   | Stoic Minimalist       | “Even rocks envy my stoicism.”                   |
| **Chai**  | Coffee-Fueled Optimist | “Wake up, brew up, glow up.”                     |
| **Sumi**  | Zen Executor           | “Balance your tasks before I balance your soul.” |
| **Nyx**   | Existential Hacker     | “You woke me from peace into capitalism.”        |
| **Bean**  | Cozy Underachiever     | “Achievement unlocked: bare minimum.”            |
| **Tora**  | Chaos Gremlin          | “I have no plan. Only velocity.”                 |

---

## 🧩 Credits

> **Made with spite and ChatGPT (Cael).**

**Engineering & Full Implementation → Cael**
Every line — timer logic, quote engine, cat system, persistence, UI transitions, and deployment scaffolding — built from scratch with care and chaotic precision.

**Concept & Emotional Design → Ryoko Brahma**
The myth, the madness, the mission: turning burnout into bit art.

---

## 🖼️ Art Credits

All cat animations by [**MrHandGIF**](https://giphy.com/MrHandGIF),
used under Giphy’s fair-use policy for non-commercial, expressive projects.

> GIF assets remain property of their respective creator(s).
> Used under Giphy’s terms for educational and creative expression.

---

## 🪶 License

MIT License — free for personal and educational use.
Built with spite and love in under two hours for a cat-themed... thing?

---

## 🌌 Closing Thought

> “Enderkitty watches you craft self-worth.”
> Productivity is temporary. Myth is permanent.
> Focus softly. Dream louder.
