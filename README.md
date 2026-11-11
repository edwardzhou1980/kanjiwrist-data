# Kanjiwrist kanji data

The kanji data shipped inside the **Kanjiwrist** app (Wear OS + Android phone, by Dolphin Studio), published here
because it is a derivative of Creative Commons Attribution-ShareAlike material and is shared under the same licence.

`data/kanji.tsv` — 2,211 kanji, one per line, tab-separated:

| column | meaning |
|---|---|
| kanji | the character |
| level | route level 5..1 (N5 easiest, N1 hardest; the levels of Jonathan Waller's JLPT lists, used only to order study) |
| rank | order within the level (KANJIDIC2 newspaper frequency, then stroke count) |
| strokes | stroke count (KANJIDIC2) |
| grade | Japanese school grade (KANJIDIC2; 0 = none) |
| freq | newspaper frequency rank (KANJIDIC2; 0 = none) |
| on | on readings in katakana, `|`-separated |
| kun | kun readings in hiragana, `.` marks okurigana, `|`-separated |
| en, fr, es, pt | meanings (KANJIDIC2), `|`-separated; KANJIDIC2 "radical" entries removed |
| examples | up to 2 common words containing the kanji, `word~reading~English gloss`, `|`-separated (JMdict, priority-tagged entries whose other kanji are at the same or an easier level) |

## Sources and licences

- **KANJIDIC2** and **JMdict** — © Electronic Dictionary Research and Development Group (EDRDG),
  https://www.edrdg.org/ — used under the Creative Commons Attribution-ShareAlike 4.0 International licence
  (https://www.edrdg.org/edrdg/licence.html). Versions: KANJIDIC2 database_version 2026-315; JMdict_e of 2026-11-11.
- **JLPT level lists** — Jonathan Waller, http://www.tanos.co.uk/jlpt/ (CC BY). The level of each kanji was taken from the
  `jlpt_new` field of https://github.com/davidluzgouveia/kanji-data (MIT), which reproduces Waller's lists. No other
  field of that repository is used.

JLPT is a test run by the Japan Foundation and JEES; this data and the app are not affiliated with or endorsed by them.
The "N5..N1" levels are unofficial lists.

**Changes made:** selection of the 2,211 kanji in the level lists, ordering, truncation of readings and meanings,
selection of example words, conversion to TSV.

## Licence

This data is licensed under **CC BY-SA 4.0** (see `LICENSE`). If you use it, credit EDRDG (KANJIDIC2, JMdict),
Jonathan Waller (level lists) and this repository, and share your changes under the same licence.

The Kanjiwrist app's code is not part of this repository and is not covered by this licence.
