# Full Korean–Russian dictionary for Namu (krdict-full.db.gz)

**Source:** 한국어기초사전 (Basic Korean Dictionary), National Institute of Korean
Language (국립국어원), https://krdict.korean.go.kr. Copied from the XML mirror at
https://github.com/spellcheck-ko/korean-dict-nikl-krdict (commit `e7249562dca526461a347eb2cc5a2e67a17c4488`).

**License:** Creative Commons Attribution-ShareAlike 2.0 Korea (CC BY-SA 2.0 KR),
https://creativecommons.org/licenses/by-sa/2.0/kr/. This file is a derivative work and
is distributed under the same license.

**Changes made by Namu:** converted from XML to SQLite (gzip-compressed) by
`scripts/build-dictionary.py --full` in https://github.com/SmaxsupeR/namu-app.
Kept: headwords, homonym numbers, parts of speech, learner levels, hanja/origin,
pronunciation, topic and subject categories, usage notes, sentence patterns, the
Russian equivalent and Russian explanation of each sense, Korean definitions, every
example (phrases, sentences, dialogues), related words and inflected forms.
Dropped: equivalents in languages other than Russian, senses without a Russian
equivalent, pictures and links to recorded pronunciation (whose redistribution is
not allowed). A search index of Russian terms was added. Two XML defects in the
source (control characters, an unescaped "<") were repaired.

Namu checks the SHA-256 of both the download and the unpacked database.
