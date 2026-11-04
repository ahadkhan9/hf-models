# Hugging Face Models (`hf-models`)

A repository for storing and hosting quantized GGUF models from Hugging Face.

## Models Included

### 1. Parakeet Unified EN 0.6B (Q8_0)

- **Filename**: `parakeet-unified-en-0.6b-Q8_0.gguf`
- **Architecture**: Parakeet Conformer RNNT (Speech-to-Text / Automatic Speech Recognition)
- **Base Model**: [nvidia/parakeet-unified-en-0.6b](https://huggingface.co/nvidia/parakeet-unified-en-0.6b)
- **Quantized By**: [handy-computer/parakeet-unified-en-0.6b-gguf](https://huggingface.co/handy-computer/parakeet-unified-en-0.6b-gguf)
- **Quantization Type**: `Q8_0` (8-bit quantization)
- **File Size**: ~731 MB (697.48 MiB)
- **Engine / Runtime**: Compatible with [transcribe.cpp](https://github.com/bingbangboom-lab/transcribe.cpp) and related GGUF speech runtimes.

#### Benchmark Quality
- **LibriSpeech test-clean WER**: ~1.60%
- **FLEURS en WER**: ~3.99%

## Git LFS Requirement

Because model files exceed GitHub's standard 100 MB file limit, this repository uses [Git Large File Storage (LFS)](https://git-lfs.com/).

To clone this repository and fetch the weights:

```bash
# Install git-lfs if not already installed
git lfs install

# Clone the repository
git clone https://github.com/ahadkhan9/hf-models.git
cd hf-models
git lfs pull
```

## License & Attribution

- Base weights by NVIDIA Corporation under the NVIDIA Open Model License.
- GGUF quantization by handy-computer.
