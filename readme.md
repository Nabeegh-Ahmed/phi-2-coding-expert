# Phi-2 Coding

This repository contains a version of Phi-2 fine tuned specifically for coding tasks.

## Overview

This model builds upon Phi-2 by Microsoft and it is fine tuned on <a href="https://huggingface.co/datasets/lucasmccabe-lmi/CodeAlpaca-20k">CodeAlpaca-20k</a> dataset. This model is fine tuned for coding purposes.

Phi-2 is not a RLHF tuned LLM. This fine tuning also adds small chat capabilities to the LLM using `Human: <prompt> Assistant:` paradigm.

## Features

- **Enhanced Domain Specificity**: Improved accuracy and relevance in coding.
- **Implementation of QLoRA**: Used QLoRA with 4-bit quantization for fine tuning

## Requirements

To use this fine-tuned model, ensure you have the following:

- Python 3.8 or later
- Run the cells in the notebook

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Nabeegh-Ahmed/phi-2-coding-expert.git
   ```
2. Run the last two cells of the notebook for inference

## Caveats

- I had very limited access to GPUs so fine tuning even on a small dataset took a huge amount of time.
- For the same reason, I was not able to fine tune on the whole dataset with short batch sizes. I only fine tuned on a small dataset to prevent CUDA out of memory errors.

## License

This project is licensed under the terms of the MIT license.

## Acknowledgements

This model is based on the work of <a href="https://huggingface.co/microsoft/phi-2">Microsoft</a>. We thank them for their foundational contributions to the field of AI and language understanding.
