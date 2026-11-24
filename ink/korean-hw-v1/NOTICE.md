# Namu handwriting model — korean-hw v1

Offline recognition of handwritten Korean for Namu's handwriting exercises.

- **Model:** `rec.onnx` is `rec_korean_hw.onnx` from
  [VerifiedIdiot/korean-handwriting-rec](https://github.com/VerifiedIdiot/korean-handwriting-rec),
  a PP-OCRv5 Korean text recogniser fine-tuned on handwritten Hangul. Unchanged.
  Licence: Apache-2.0 (see `LICENSE`).
- **Character list:** `dict.txt` is `ppocrv5_korean_dict.txt` from the same repository
  (from PaddleOCR, Apache-2.0). Model output classes: blank, these characters, space.
- **Training data:** the fine-tuning used AI Hub datasets (Korea, NIA), which have their own
  terms of use; the data itself is not included here.
- **Base model:** [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) PP-OCRv5, Apache-2.0.

Namu runs this model on the phone with ONNX Runtime; nothing written by the user leaves the device.
