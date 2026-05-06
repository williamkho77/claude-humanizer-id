# humanizer-bahasa-Indonesia

A [Claude Code](https://claude.ai/code) skill that removes AI writing patterns from Indonesian text and rewrites it to sound natural and human.

Based on the same approach as [blader/humanizer](https://github.com/blader/humanizer) (for English), but rebuilt from scratch for Bahasa Indonesia — covering patterns specific to how LLMs write Indonesian.

## What it fixes

- **Merupakan overuse** — AI's way of avoiding plain "adalah"
- **AI vocabulary** — sangat penting, krusial, holistik, inovatif, revolusioner, komprehensif
- **Vague attributions** — para ahli, studi menunjukkan, beberapa sumber
- **Filler phrases** — perlu diketahui bahwa, dalam konteks ini, dengan demikian
- **Excessive hyphens** — the Indonesian equivalent of em dash abuse
- **Inconsistent register** — mixing formal Bahasa baku with casual in the same paragraph
- **Passive voice overuse** — di- constructions when active is more natural
- **Promotional language** — revolusioner, mutakhir, terdepan, memukau
- **Generic conclusions** — Dengan demikian kita dapat menyimpulkan..., Ke depannya diharapkan...
- **Chatbot artifacts** — Semoga bermanfaat!, Jangan ragu untuk bertanya
- **Negative parallelism** — tidak hanya... tetapi juga...
- **Signposting** — Mari kita telaah..., Tanpa basa-basi lagi
- **Rule of three overuse**, **overlong chained sentences**, **excessive hedging**, and more

## Install

```bash
git clone https://github.com/williamkho77/claude-humanizer-id.git ~/.claude/skills/humanizer-bahasa-Indonesia
```

Then restart Claude Code.

## Usage

```
/humanizer-bahasa-Indonesia

[paste your text here]
```

The skill will ask for your target register (formal / semi-formal / kasual) before rewriting. It then produces:

1. A draft rewrite
2. A self-critique — "what still makes this feel AI-generated?"
3. A final revised version
4. A summary of changes

## Voice matching

You can provide a sample of your own writing to match your personal style:

```
/humanizer-bahasa-Indonesia

Ini contoh tulisan saya untuk referensi gaya:
[tempel tulisanmu sendiri di sini]

Sekarang humanisasi teks ini:
[teks yang ingin diubah]
```

## Credits

Built by [@williamkho77](https://github.com/williamkho77) with Claude Code.
Inspired by [blader/humanizer](https://github.com/blader/humanizer) and [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).
