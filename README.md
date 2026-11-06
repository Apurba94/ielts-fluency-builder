# Fluency Builder

Speak on a topic without stopping for one or two minutes, record it, and track how long you keep going.

Part of the [IELTS Study Suite](https://github.com/Apurba94/ielts-study-suite): 100 free study apps for IELTS. This one is for the IELTS Academic and General Training test. It works offline, as a Windows program or in the browser.

## Download and run

- **Windows:** download `Fluency Builder.exe` from the [latest release](https://github.com/Apurba94/ielts-fluency-builder/releases/latest) and open it. Nothing to install. It opens in its own window and saves your progress in your user folder.
- **Browser:** open it online in the suite's web edition at https://ielts-study-suite.vercel.app/apps/ielts-fluency-builder/ . Progress stays in that browser.
- **From source:** `python launcher.py` (Python 3.10 or later, no packages needed).

## What it does

Fluency is a quarter of your Speaking score: keeping going without long pauses, and linking ideas as you speak. Get a random topic from the Part 2 cards, speak for one or two minutes without stopping, and record yourself. Then listen back and count long pauses and fillers such as um and er. The chart should show fewer of both over time.

Sections: Practice, Progress, About.

## How to use it

1. Choose one or two minutes and press **New topic**. You get 15 seconds to think.
2. Speak until the time is up. Keep going even if you make mistakes.
3. Listen back and enter your counts honestly. The score is a self-check, not an IELTS band.

## Good to know

- All questions, passages, recordings and definitions were written for this suite. None are official IELTS questions. For official practice, use the materials on ielts.org and from the test partners.
- It follows IELTS as delivered on computer in 2026. Formats change, so check ielts.org before your test.
- Listening uses the voices installed on your computer, which sound less natural than real test recordings.
- Feedback on writing and speaking counts what a program can count honestly, such as length and linking words. It is not an IELTS band score. Band conversions for Listening and Reading are approximate.
- Not endorsed by or affiliated with the British Council, IDP or Cambridge University Press & Assessment. IELTS is a registered trademark of its owners.

## For developers

The app is plain HTML and JavaScript in `web/`, run by a small Python launcher that serves it on 127.0.0.1 only and needs a secret token for saving. Tests: `node --test "tests/*.test.js"` (29 tests) and `python -m unittest discover -s tests`. Build the .exe with `python build_exe.py`.

Built with AI assistance (Claude Code). MIT licence. By JANIN A APURBA.
