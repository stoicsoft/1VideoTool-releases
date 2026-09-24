# 1VideoTool

**From script to shots to final cut, in folders you own.**

1VideoTool is a local-first AI video studio for macOS. Describe a video or paste a
screenplay, and it breaks the story into scenes and shots. It makes the pictures, voices
the narration, cuts to the music, masters the sound, and hands you a finished MP4. It
checks the result before it calls it done.

- **Your coding agent directs it.** The writing is done by the CLI you already use:
  Claude Code, Codex, Gemini CLI, Cursor Agent, OpenCode, Qwen, Grok, Devin or Aider. You
  approve the script and the final cut, or let the run go straight through.
- **Your keys, your bill.** Stills and motion from Gemini (Nano Banana, Veo), Runway and
  fal go through API keys you paste. Every paid call shows its estimate before it runs.
  The app sells no compute and adds no markup.
- **Local where it can be.** Motion-graphics templates, the 2D Ink engine, Blender 3D,
  narration, the mix and the master all run on your Mac.
- **Files, not an account.** A production is a folder of readable JSON, media and a
  ledger. Every take is kept. Nothing needs a login, and API keys live in the macOS
  Keychain.

## Downloads

Get the newest installer from
[**Releases**](https://github.com/stoicsoft/1VideoTool-releases/releases/latest).

| Your Mac | File |
|---|---|
| Apple Silicon (M1 and later) | `1VideoTool_<version>_aarch64.dmg` |
| Intel | `1VideoTool_<version>_x64.dmg` |

Open the `.dmg` and drag **1VideoTool** into **Applications**. Requires **macOS 13 Ventura
or later**. Windows and Linux builds are not available yet.

## Before your first video

| You need | Why | How |
|---|---|---|
| **FFmpeg** | Every render, mix, master and export | `brew install ffmpeg` ([Homebrew](https://brew.sh)). The title bar says **No FFmpeg** until it is found. |
| A coding CLI *(for director runs)* | Writes the script, the shots and the titles | Any one of those listed above, installed and signed in. The app finds it on its own. |
| Provider keys *(optional)* | AI stills and motion | Settings → Providers. Gemini, Runway, fal. Skip them and everything local still works. |
| Blender *(optional)* | The 3D route | Settings → Local rendering installs a pinned, checksum-verified build, or points to yours. |
| Local voice *(optional)* | Narration | Settings → Local voice downloads it once. After that it works offline. The macOS voice is the fallback. |

Not sure where to start? Open the bundled **Harbor Light** sample. It's a finished
12-shot production that exports a storyboard, captions and an edit list with no keys at
all.

## What you can make

**Director runs: brief to finished video.** Pick a format, describe the video, choose how
hands-on to be. Formats set the beats, the length, the aspect ratio and the checks:

| Format | Format | Format |
|---|---|---|
| Product demo | Explainer | Social ad |
| Brand film | Trailer | Music video (cut to your track) |
| Training | Documentary | From your script |

Each run writes, checks and repairs its own script. It voices the lines, renders, and
masters the loudness to a streaming target (−16 LUFS). Before the final gate it checks the
master: length against the brief, aspect ratio, loudness and peak, unintended black
frames, and motion in the opening frames.

**Three ways to make pictures:**

- **Motion graphics.** Kinetic type, charts, countdowns, timelines, product spotlights,
  before/after, collage and more. Rendered frame by frame on your Mac, with bundled fonts
  and assets.
- **Ink.** A 2D illustration and animation engine: rigs, springs, walk cycles, cel,
  watercolour and cutout styles, print filters, and an anime character pack with posable
  characters and spring-physics hair.
- **3D with Blender.** Your agent writes each shot as a scene. The app compiles it for
  Blender, renders it with Eevee or Cycles, and lip-syncs characters to the dialogue.

Add cloud stills and motion on top with your own keys, and keep every take side by side.

**Deliver.** A final MP4, a storyboard PDF, captions (SRT), an FCP7 XML edit list for
your editor, and a manifest that records the provider, prompt and file hash of every
asset.

## Free and Pro

The free tier never expires and has no trial clock.

| | Free | Pro |
|---|---|---|
| Finished-video exports | 25 | Unlimited |
| Director runs | 10 | Unlimited |
| Output | Up to 1080p, 30 fps, 3 minutes | Up to 4K, 60 fps, 10 minutes |
| End card | "Made with 1VideoTool", 2 s, can be switched off | None |
| Drafts, previews, takes, storyboards, captions, FCP7 XML | Unlimited | Unlimited |

The free tier never watermarks your footage. You paid your provider for those shots.

**Pro is one payment, not a subscription:** $29 for one Mac, $59 for three, $89 for five.
It includes 12 months of updates, and the version you have keeps working forever after
that. Buy and activate from **Settings → License**.

## Updates

The app checks this repository for new versions and installs them from **Settings →
Updates**. Every update is signed, and the app refuses one that isn't. Only published
releases are served; drafts are not.

## Privacy

- Productions, media and logs stay on your disk.
- API keys stay in the macOS Keychain. They never go into a production folder, a
  manifest or an agent prompt.
- Anonymous usage counts are off until you say yes, and can be turned off in
  **Settings → Privacy**. They never include your scripts, prompts, footage, file names or
  keys.

## Troubleshooting

- **"1VideoTool can't be opened" / "unidentified developer".** Right-click the app →
  **Open** → **Open** once. Later signed releases won't ask.
- **No FFmpeg** in the title bar. Run `brew install ffmpeg`, then restart the app.
- **The agent isn't listed.** Check that the CLI runs in Terminal and is signed in, then
  press **Rescan Blender & CLIs** in Settings.

## Issues

This repository holds the release files; the source lives elsewhere. File bugs and
requests in [Issues](https://github.com/stoicsoft/1VideoTool-releases/issues). Include
your macOS version, your Mac's chip, and the app version from Settings.
