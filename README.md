# Flappy Heart

A medical take on Flappy Bird. You're a winged heart flying down a hospital corridor. Every flap is a heartbeat: dodge the syringes, grab the pills, and keep the pulse going.

## How to play

- **Flap:** click, tap, or press `Space` / `↑` / `W`
- **Mute all sound:** the speaker button, or press `M`
- **Music on/off:** the music-note button, or press `N`
- Get past a syringe for **+1**, and grab a pill for another **+1**
- Hit a needle or the floor and you flatline. Tap to charge the defibrillator and get back in.

## Features

- **Bedside monitor.** A live ECG trace draws a PQRST complex every time you flap. The heart rate in bpm comes from your real flap rhythm, so panic-flapping triggers a *TACHYCARDIA* warning. When you die, it switches to *ASYSTOLE*.
- **Hospital corridor.** Wards, windows, notice boards and a wall clock that shows your real local time scroll past with parallax.
- **Patient chart game over.** The game-over screen is a patient chart with your score, your best, and a condition rating from *Critical* up to *Chief of Medicine*.
- The game gets harder as you score: it speeds up and the gaps between needles shrink.
- **Sound and music.** Everything is generated live with the Web Audio API, so there are no audio files:
  - An 8-bar chiptune loop plays throughout. Drums come in when you start flying, and the tempo rises as the game speeds up.
  - Underneath is a quiet hospital hum, with an occasional "ding-dong" from the overhead PA.
  - Each flap plays a monitor beep and a heartbeat thump. On the title screen, the heart beats "lub-dub".
  - You hear a chime and a whoosh for each syringe you pass, a sparkle for each pill, a "shing" for a close call past a needle tip, and fanfares at every 10 points and when you beat your record.
  - Flapping too fast sets off a tachycardia alarm.
  - Hitting a needle makes a metallic tink. Then comes the flatline tone, the paper slide of the patient chart, and a defibrillator that whines as it charges, fires with a zap, and plays a revive chime.
- Works on phones and desktops, sharp on high-DPI screens, and honors reduced-motion settings.
- Your best score is saved in your browser.

## Run it

Everything is in one `index.html` file with no build step and no dependencies. Fonts come from Google Fonts, and the game falls back to system fonts when they can't load.

- **Locally:** open `index.html` in a browser.
- **GitHub Pages:** push this folder to a repo, then go to **Settings → Pages → Deploy from a branch**, pick `main` and `/ (root)`, and save. The game will be live at `https://<your-username>.github.io/<repo-name>/`.
