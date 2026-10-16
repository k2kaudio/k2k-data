# k2k-data

Data files and models that K2K Editor downloads on first use. The app shows each file's licence before
downloading it and checks its SHA-256. Nothing here is needed to build the app.

## Releases

### `bsrnn-simo-v1` — Band-Split RNN stem model (StemSplit node)

| | |
|---|---|
| File | `bsrnn_simo.onnx` (436,887,727 bytes) |
| SHA-256 | `db269f1ee0a1739409f40e88d7b1fde02713c9f0ee45a87430b772a2cadb479b` |
| Model | oBSRNN-SIMO — P. Magron, R. Serizel, C. Douwes (Inria), https://github.com/magronp/bsrnn (code: MIT) |
| Weights | https://zenodo.org/records/17516442 — licence **CC BY 4.0** (https://creativecommons.org/licenses/by/4.0/) |
| Changes | Exported to ONNX (opset 17, fp32) and simplified with onnxsim by K2K Audio; network weights unchanged. |
| Note | The model was trained on the MUSDB18-HQ dataset. |
