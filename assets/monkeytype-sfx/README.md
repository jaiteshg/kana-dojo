# Monkeytype SFX Export

This directory contains Monkeytype website sound-effect WAV files exported from:

- Repository: https://github.com/monkeytypegame/monkeytype
- Source folder: `frontend/static/sound`
- Reference source: `frontend/src/ts/controllers/sound-controller.ts`

Selection rule:

- Includes all `.wav` files referenced by Monkeytype's sound controller.
- Preserves original filenames and subfolder structure.
- WAV-only export (no transcoding).

Regeneration (PowerShell):

1. Fresh-clone Monkeytype to `C:\Users\reser\monkeytype`.
2. Parse `sound-controller.ts` for `../sound/...wav` references.
3. Copy those files from `frontend/static/sound` to this directory.
4. Rebuild `manifest.json`.

## Credits

### Sponsor

- [Vercel](https://vercel.com/) — KanaDojo is supported by Vercel.
- [Vercel Open Source Program](https://vercel.com/open-source-program) — part of the broader OSS ecosystem we’re grateful to be included in.

### Inspiration

- [Duolingo](https://www.duolingo.com/) — learning-game inspiration.
- [Monkeytype](https://monkeytype.com/) — typing-practice inspiration.
- [Monkeytype GitHub repository](https://github.com/monkeytypegame/monkeytype) — source of the exported sound effects in this folder.

### Japanese Language Libraries

- [Kuroshiro](https://github.com/hexenq/kuroshiro) — Japanese text conversion and romanization.
- [Kuromoji](https://github.com/takuyaa/kuromoji.js) — Japanese tokenizer used for text analysis.
- [Wanakana](https://github.com/WaniKani/WanaKana) — kana and romaji transliteration helpers.

### Data Sources

- [JMdict](https://www.edrdg.org/jmdict/j_jmdict.html) — Japanese-English dictionary data.
- [KANJIDIC](http://www.edrdg.org/wiki/index.php/KANJIDIC_Project) — kanji readings and meanings database.
- [Jonathan Waller's JLPT Resources](https://japanesetest4you.com/) — JLPT study references.
- [jlptsensei.com](https://jlptsensei.com/) — JLPT vocabulary and study material.
