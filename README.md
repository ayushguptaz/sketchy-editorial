# Sketchy Editorial — Claude Code Plugin

A Claude Code skill that generates **minimalist hand-drawn editorial illustrations** for English articles, blog posts, slide decks, and documentation.

## What It Does

Turns your article's key ideas into 16:9 minimalist hand-drawn illustrations featuring a recurring solid-black ink character that seriously performs absurd-but-logical actions to explain concepts visually.

**Style:** pure white background, black ink sketch, sparse red/orange/blue handwritten annotations, lots of white space, deadpan humor, never cute.

## Installation

### Via Claude Code CLI

```bash
claude plugin add <your-github-username>/sketchy-editorial
```

### Manual Installation

Clone this repo and symlink the skill:

```bash
git clone https://github.com/<your-username>/sketchy-editorial.git
ln -s /path/to/sketchy-editorial/skills/sketchy-editorial ~/.claude/skills/sketchy-editorial
```

## Usage

In Claude Code, invoke the skill:

```
/sketchy-editorial
```

Or describe what you want:

- "Generate illustrations for this blog post about microservices"
- "Create a shot list for my article on context windows in LLMs"
- "Make 4 editorial sketches for my slides about distributed systems"

## What You Get

1. **Shot list** — placement, theme, core meaning, structure type, character role, suggested elements and labels
2. **Generation prompts** — ready to paste into any image generator (DALL-E, Midjourney, Gemini, etc.)
3. **Direct generation** — if you have an image generation MCP server connected, images are created automatically

## Requirements

- Claude Code CLI or IDE extension
- (Optional) An image generation MCP server (e.g., `gemini-image-gen`, `dall-e`) for automatic generation

## Style Rules

- One image = one core concept
- The ink character performs the action (not decoration)
- Absurd but logical metaphors
- Maximum 5-8 short English labels
- At least 35% white space
- No PPT, no flowcharts, no cute cartoons

## License

MIT
