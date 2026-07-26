# My Tools

A collection of small offline browser tools — each is a single self-contained
HTML file (no build step, no dependencies, no backend).

## Tools included

| File | Description |
|---|---|
| `index.html` | Homepage linking to all tools |
| `interview_simulator.html` | Mock interview practice — voice input, timer, AI feedback, history |
| `excuse_generator.html` | Random excuse generator with voice playback |
| `insult_to_compliment.html` | Turns any typed line into a funny backhanded compliment |
| `battle_bot.html` | Random compliment / roast generator |
| `debate_practice_bot.html` | Random for/against arguments on a topic |
| `horoscope_randomizer.html` | Funny random horoscope generator |
| `fake_call.html` | Simulated incoming call screen |
| `virtual_pet.html` | Simple virtual pet you can feed/play with |

## Deploy to GitHub + Vercel

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit — my tools"
git branch -M main
git remote add origin https://github.com/MubasharAkram05/YOUR-REPO-NAME.git
git push -u origin main
```
(Replace `YOUR-REPO-NAME` with whatever you name the repo on GitHub.)

### 2. Deploy on Vercel
1. Go to https://vercel.com and sign in with your GitHub account.
2. Click **Add New → Project**.
3. Select this repository.
4. Framework preset: choose **Other** (this is plain static HTML, no build needed).
5. Leave build command and output directory empty/default.
6. Click **Deploy**.

Vercel will give you a live URL like `https://your-repo-name.vercel.app` —
open it on your phone and every tool works directly, including microphone
input (voice-to-text), since Vercel serves everything over HTTPS.

### Notes
- No environment variables or API keys are required for any tool except
  `interview_simulator.html`'s optional **AI Feedback** feature, which asks
  the user to paste their own Anthropic API key at runtime (never stored,
  never committed to the repo).
- Do **not** hardcode any API key into these files before pushing to GitHub —
  the repo may be public.
