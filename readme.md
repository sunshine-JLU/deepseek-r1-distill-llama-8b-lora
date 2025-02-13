## Quick Start

Follow these steps to get started quickly:

1. **Clone the Repository**  
   Clone the repository to your local machine:
   ```bash
   git clone https://github.com/sunshine-JLU/deepseek-r1-distill-llama-8b-lora.git

   cd deepseek-r1-distill-llama-8b-lora

   
2. **Enviroment**  
   ```bash
   pip install -r requirements.txt

3. **Download the Model**  
  Set the Hugging Face endpoint and download the deepseek-r1-distill-llama-8b model:
   ```bash
   HF_ENDPOINT=https://hf-mirror.com huggingface-cli download deepseek-ai/deepseek-r1-distill-llama-8b --local-dir ./deepseek-r1-distill-llama-8b --resume-download --cache-dir ./cache

   #if you have trouble in downloading models from hf-mirror, you can use the modelscope.
   
   modelscope download --model deepseek-ai/DeepSeek-R1-Distill-Llama-8B --local_dir ./deepseek-r1-distill-llama-8b


4. **Run the Notebook**  
  Open and run the deepseek-r1-distill-llama-8b.ipynb notebook to start fine-tuning the model.

5. **Run the lora-model in the lora_model_inference.ipynb**  
  After you successfully run over the deepseek-r1-distill-llama-8b.ipynb, You will get a number of checkpoint files, each file is a lora weight that can be loaded independently, you can specify the lora file address in the lora_model_inference.ipynb to load and run.
![1738867391045](https://github.com/user-attachments/assets/65530629-32fb-415f-9a8e-e3cadabb90e1)


## Hardware requirement

GPU Memory at least 48GB would not appear OOM problem.
![微信图片_20250206162602](https://github.com/user-attachments/assets/e4232a2e-4e5d-4636-921e-d9e6e4855134)

## Test Enviroment 
I deploy this program under PyTorch 2.3.0 ,Python 3.12(ubuntu22.04), Cuda  12.1
 
