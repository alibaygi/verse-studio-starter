# Setup prompt

Open an empty folder called `verse-studio` in Claude Code, put your own
`STYLE.md` in it (see the template in README.md), then paste everything below
the line.

---

I make videos and short motions about books and ideas (Instagram reels 9:16,
YouTube 16:9). This folder is my video studio. My style is in STYLE.md: read it
first and follow it in everything you design, write or edit.

1. STRUCTURE – create exactly this:
verse-studio/
  CLAUDE.md      (you write it: rules + workflows below)
  STYLE.md       (already here, my style guide; don't change it without asking)
  inkwell/fonts/  inkwell/paper/  inkwell/portraits/  inkwell/sounds/
  stamps/        (reusable scenes: title card, plate, quote card, call to action)
  margins/       (references I study)
  plates/        (one folder per video)
A new video = plates/plate-NNN_short-name/ with:
  sources/  script.md  storyboard.md  footage/  scenes/  press/
Ask me before adding any other folder.

2. TOOLS – check what's installed, tell me what you'll install, then set up and
report versions:
- Node.js 22+
- FFmpeg (cutting and export)
- Whisper (transcription and subtitles): pick the best version for my machine,
  e.g. whisper.cpp or mlx-whisper on Apple Silicon; use large-v3 or turbo if my
  hardware allows; set the language of my videos
- yt-dlp (downloading reference videos, for study only)
- Remotion (assembling videos from code)
- HyperFrames (motion graphics), installed as a Claude Code plugin:
  claude plugin marketplace add heygen-com/hyperframes
  claude plugin install hyperframes@hyperframes
Download the fonts named in STYLE.md into inkwell/fonts/.

3. WORKFLOWS – save them in CLAUDE.md
New plate from an article, a link or notes:
  sources → script.md (I edit) → storyboard.md (I approve) →
  scenes in HyperFrames following STYLE.md → preview → render to press/
Editing my recording:
  footage → transcript (I correct) → cut list (I approve) →
  subtitles in my style → export to press/ → suggest 3–4 short clips
Stamps: when a scene works well, offer to save it in stamps/ for reuse.

4. RULES – save them in CLAUDE.md
- Never edit, move or delete anything in footage/.
- margins/ is for studying only: never reuse other people's footage, music or
  voice.
- Ask before renders longer than a few minutes.
- Right-to-left text (Farsi, Arabic, Hebrew) is rendered in the browser
  (HyperFrames/Remotion), never with FFmpeg drawtext.

5. FIRST TASK
Set everything up, then build stamps/title-card: 5 seconds, 1080×1920, a short
line of my choice writing itself on the paper colour from STYLE.md. Render it to
stamps/title-card/press/ and stop. Report back to me.
