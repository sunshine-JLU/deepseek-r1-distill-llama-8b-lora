Quick Start
Follow these steps to get started quickly:
Clone the Repository
Clone the repository to your local machine:
bash
复制
git clone https://github.com/sunshine-JLU/deepseek-r1-distill-llama-8b-lora.git
Download the Model
Set the Hugging Face endpoint and download the deepseek-r1-distill-llama-8b model:
bash
复制
HF_ENDPOINT=https://hf-mirror.com
huggingface-cli download deepseek-ai/deepseek-r1-distill-llama-8b \
  --local-dir ./deepseek-r1-distill-llama-8b \
  --resume-download --cache-dir ./cache
Run the Notebook
Open and run the deepseek-r1-distill-llama-8b.ipynb notebook to start fine-tuning the model.
