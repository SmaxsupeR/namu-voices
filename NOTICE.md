# NOTICE

The voice packs in this repository are modified versions ("Derivatives of the Model") of
**Supertonic 3** by **Supertone Inc.** — <https://huggingface.co/Supertone/supertonic-3>,
commit `3cadd1ee6394adea1bd021217a0e650ede09a323` — licensed under the
**BigScience OpenRAIL-M License** ([LICENSE](LICENSE)).

## Changes

Made by the Namu project, 2026-11-17, for pack `int8w`:

- `onnx/duration_predictor.onnx`, `onnx/text_encoder.onnx`, `onnx/vector_estimator.onnx`,
  `onnx/vocoder.onnx`: the weights of Conv, MatMul and Gemm layers are stored as INT8
  (symmetric, per output channel) and expanded back to float32 by `DequantizeLinear` nodes
  when the model is loaded. The network architecture is unchanged. Each modified file
  carries `modified_by`, `modification`, `original_model` and `license` metadata.
- `onnx/tts.json`, `onnx/unicode_indexer.json` and `voice_styles/*.json` are unchanged copies.

## Use-based restrictions

Paragraph 5 and Attachment A of the License apply to every pack here and to every use of it.
By downloading or using a pack you agree to them. Among other things, you must not use the
model or its outputs:

- in any way that violates applicable law;
- to impersonate or attempt to impersonate others without their consent (e.g. deepfakes);
- to generate or disseminate content without expressly disclosing that it is machine-generated;
- to defame, harass or harm others, or to exploit or harm minors;
- for the other restricted uses listed in Attachment A of the [LICENSE](LICENSE).

Anyone you pass a pack on to must receive the License and must be bound by the same restrictions.
