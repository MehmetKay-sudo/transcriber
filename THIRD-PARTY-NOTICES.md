# Third-party components

The packages bundle the following components with their own licenses.
The MIT license in `LICENSE` covers Transcriber's own code only.

| Component | License | Source |
|---|---|---|
| Python 3.14 | PSF-2.0 | https://www.python.org |
| Tcl/Tk 8.6 | Tcl/Tk license (BSD-style) | https://www.tcl-lang.org |
| PyInstaller bootloader | GPL-2.0 with bootloader exception | https://pyinstaller.org |
| faster-whisper 1.2.1 | MIT | https://github.com/SYSTRAN/faster-whisper |
| CTranslate2 4.9.1 | MIT | https://github.com/OpenNMT/CTranslate2 |
| onnxruntime 1.32.0 | MIT | https://github.com/microsoft/onnxruntime |
| PyAV 19.0.2 (with bundled FFmpeg libraries) | BSD-3-Clause; FFmpeg: LGPL-2.1+ | https://github.com/PyAV-Org/PyAV · https://ffmpeg.org |
| tokenizers 0.23.3 | Apache-2.0 | https://github.com/huggingface/tokenizers |
| huggingface_hub 2.4.0 | Apache-2.0 | https://github.com/huggingface/huggingface_hub |
| hf-xet 1.8.0 | Apache-2.0 | https://github.com/huggingface/xet-core |
| fpdf2 2.9.0 | LGPL-3.0-only | https://github.com/py-pdf/fpdf2 |
| fonttools 4.68.0 | MIT | https://github.com/fonttools/fonttools |
| Pillow 13.0.0 | MIT-CMU | https://github.com/python-pillow/Pillow |
| NumPy 2.5.5 | BSD-3-Clause and others | https://numpy.org |
| psutil 7.2.2 | BSD-3-Clause | https://github.com/giampaolo/psutil |
| protobuf 7.36.2 | BSD-3-Clause | https://github.com/protocolbuffers/protobuf |
| flatbuffers 25.12.19 | Apache-2.0 | https://github.com/google/flatbuffers |
| tqdm 4.70.1 | MPL-2.0 and MIT | https://github.com/tqdm/tqdm |
| httpx2 / httpcore2 2.16.2, idna, click, fsspec | BSD-3-Clause | PyPI |
| anyio, h11, filelock, PyYAML, truststore | MIT | PyPI |
| packaging | Apache-2.0 or BSD-2-Clause | PyPI |
| typing_extensions | PSF-2.0 | PyPI |

The macOS package additionally bundles:

| Component | License | Source |
|---|---|---|
| PyTorch 2.15.0 | BSD-3-Clause | https://github.com/pytorch/pytorch |
| openai-whisper 20250625 | MIT | https://github.com/openai/whisper |
| tiktoken 0.14.0 | MIT | https://github.com/openai/tiktoken |
| numba 0.68.1, llvmlite 0.50.0 | BSD-2-Clause (llvmlite bundles LLVM: Apache-2.0 with LLVM exception) | https://numba.pydata.org |
| regex 2026.11.23 | Apache-2.0 | https://github.com/mrabarnett/mrab-regex |
| sympy 1.14.0, mpmath 1.3.0, networkx 3.7 | BSD-3-Clause | PyPI |
| Jinja2 3.1.6, MarkupSafe 3.0.4 | BSD-3-Clause | PyPI |
| more-itertools 11.2.1 | MIT | PyPI |

The Whisper speech models are not bundled. They are downloaded on first use
from Hugging Face and are published by OpenAI under the MIT license.
