# Chinese Zodiac Dataset

A clean, structured JSON dataset of the 12 Chinese zodiac animals (生肖 / Shēngxiào) with traditional Chinese names, pinyin, Earthly Branches, fixed elements, years, branch hours, and traditional trait associations.

Used by [I Ching Master Li](https://www.askmasterli.com/), a free AI-powered I Ching reading platform that casts hexagrams with the traditional three-coin method and explains the moving lines, BaZi (Four Pillars), and Feng Shui.

👉 [Discover your Chinese zodiac sign and 2026 fortune (free, no signup)](https://www.askmasterli.com/zodiac)

## Files

- `zodiac.json` — all 12 animals in zodiac order, with year ranges 1900–2036.

## Data Fields

Each animal object contains:

| Field | Description |
|---|---|
| `number` | Zodiac order (1–12), starting with Rat |
| `animal` | English name |
| `chinese` | Simplified Chinese character |
| `pinyin` | Mandarin pronunciation |
| `earthly_branch` | Corresponding Earthly Branch (地支), Chinese + pinyin |
| `fixed_element` | Fixed element: Wood, Fire, Earth, Metal, or Water |
| `polarity` | Yin or Yang |
| `branch_hours` | Traditional branch time window |
| `years` | Lunar years associated with the sign (1900–2036) |
| `traditional_traits` | Traditional positive and challenging trait associations |

Example:

```json
{
  "number": 7,
  "animal": "Horse",
  "chinese": "马",
  "pinyin": "Mǎ",
  "earthly_branch": { "chinese": "午", "pinyin": "Wu" },
  "fixed_element": "Fire",
  "polarity": "yang",
  "branch_hours": "11:00–13:00",
  "years": [1918, 1930, 1942, 2014, 2026],
  "traditional_traits": {
    "positive": ["energetic", "independent", "sociable", "adventurous"],
    "challenges": ["restless", "impatient"]
  }
}
```

## Important Note: Chinese New Year Boundary

Years in this dataset follow the **Chinese lunar calendar**, not the Gregorian year. Each zodiac sign begins on Chinese New Year (which falls between late January and mid-February). Someone born in January or early February may belong to the **previous** year's sign. Always verify the exact New Year date for boundary birthdays.

## More Free Tools

- [Kua number calculator, zodiac compatibility & I Ching coin casting](https://www.askmasterli.com/tools) — free, no signup
- [Free AI I Ching reading](https://www.askmasterli.com/) — 3 free readings per day

## Disclaimer

Trait descriptions are traditional cultural associations for entertainment and personal reflection only. They are not personality assessments, predictions, or professional advice. For entertainment purposes only.

## License

MIT — free for personal and commercial use. Attribution appreciated but not required.

---

> 本内容由 Coze AI 生成，请遵循相关法律法规及《人工智能生成合成内容标识办法》使用与传播。
