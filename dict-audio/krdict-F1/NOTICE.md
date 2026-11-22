# Namu dictionary audio — krdict, voice F1

Pre-recorded pronunciation of every headword of 한국어기초사전 (Basic Korean
Dictionary, National Institute of Korean Language) that the Namu app ships:
41 663 recordings in one voice (F1).

- **Machine-generated speech.** Every clip was synthesised with Supertonic 3
  (Supertone), Namu voice pack `int8w` v2 (INT8 weights, FP16 vocoder),
  8 steps, speed 1.0, seed 42, peak-normalised to −1 dBFS. No human recorded it.
- **Model licence:** BigScience OpenRAIL-M. Its use restrictions apply to these
  recordings too; disclose that the speech is machine-generated.
- **Texts:** headwords of 한국어기초사전, CC BY-SA 2.0 KR, read in their main
  variant (optional parts like `(가)` kept, alternatives after `/` dropped).
- **Format:** one SQLite database `audio(text PRIMARY KEY, data BLOB)` +
  `meta`, page size 64 KiB, WebM/Opus mono 32 kbit/s. Split into parts of at
  most 45 MiB (`part00`…); concatenate them in order. `manifest.json` lists the
  SHA-256 of every part and of the whole file.
