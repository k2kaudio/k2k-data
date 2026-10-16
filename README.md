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

### `onnxruntime-cuda-1.31.0` — ONNX Runtime CUDA provider (Linux x64, GPU pack)

Part of K2K Editor's optional "GPU acceleration for NVIDIA" download. The NVIDIA libraries it needs (CUDA runtime,
cuBLAS, cuRAND, cuDNN) are **not** hosted here: the app downloads them from NVIDIA's official packages on PyPI and
shows NVIDIA's licence first.

| File | Bytes | SHA-256 |
|---|---|---|
| `libonnxruntime_providers_cuda.so.gz` | 436,613,559 | `c5186adc58eeab7af7b468504f6eac37c01a596c01ca500e4851b0bd31a02c6c` |
| `libonnxruntime_providers_shared.so.gz` | 1,717 | `ec7c2d8057213f61e146b198fad1bacbb2a3f27cbd3c885cb1530290e4d8e59d` |

Unmodified (gzip only) from the official `onnxruntime-linux-x64-gpu_cuda12-1.31.0.tgz`
(https://github.com/microsoft/onnxruntime/releases/tag/v1.31.0). ONNX Runtime © Microsoft Corporation, MIT licence
(https://github.com/microsoft/onnxruntime/blob/main/LICENSE).
