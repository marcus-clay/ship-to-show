# Ship to Show

A Claude Code skill that transforms prototypes into portfolio case studies with animated videos, narrative content, and integration packs.

## What it produces

From a working prototype (React, Vue, HTML, exported Figma), Ship to Show produces:

- A bilingual case study (FR/EN) with narrative structure
- 5 to 8 animated videos (Late Checkout Agency style: autoplay, loop, dark background)
- Retina screenshots of the prototype
- A prototype deployed on Vercel (public URL)
- A GitHub repository
- A self-contained integration pack for the portfolio site

## The 7 phases

1. **CADRER** (15 min) : Identify sector, users, problem, design hypothesis
2. **STRUCTURER** (10 min) : Make the prototype runnable locally
3. **ENRICHIR** (30-45 min) : Add missing user flows for 5 demo videos
4. **FILMER** (30 min) : Produce videos via Puppeteer + FFmpeg
5. **RACONTER** (20 min) : Write the case study with narrative structure and video captions
6. **EMPAQUETER** (15 min) : GitHub, Vercel, self-contained integration file
7. **PUBLIER** (variable) : Integrate into the portfolio site

Total: approximately 2h30 for a complete published case study.

## Prerequisites

- Node.js 18+
- FFmpeg (`brew install ffmpeg`)
- Git
- GitHub CLI (`brew install gh`)
- Vercel CLI (`npm i -g vercel`)
- Claude Code (or equivalent AI coding agent)

## Installation

```bash
mkdir -p ~/.claude/skills/ship-to-show
curl -o ~/.claude/skills/ship-to-show/SKILL.md \
  https://raw.githubusercontent.com/marcus-clay/ship-to-show/main/SKILL.md
```

## Usage

In any Claude Code project, type:

```
/ship-to-show
```

Claude Code will load the skill and execute the 7 phases sequentially on the current project.

## Example

This framework was designed and tested on [RiskOS](https://github.com/marcus-clay/riskos-fraud-detection), a fraud detection prototype with agentic AI interfaces. The published case study is available at [victorsoussan.fr/fr/project/riskos/summary](https://www.victorsoussan.fr/fr/project/riskos/summary).

## License

MIT

## Author

Victor Soussan / [Condamine Studio](https://www.victorsoussan.fr)
