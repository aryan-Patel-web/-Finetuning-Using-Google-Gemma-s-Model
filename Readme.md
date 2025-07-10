

# Gemma-LoRA-FineTuning

Fine-tune Google’s Gemma LLM using LoRA adapters on an English quotes dataset.

This repo shows:
- Loading Google Gemma with 4-bit quantization
- Preparing data with HuggingFace Datasets
- Efficient LoRA fine-tuning with TRL’s SFTTrainer
- Generating new text in the style of famous quotes

---

## 🚀 How to Run

### 1. Install Requirements

```bash
pip install -U bitsandbytes==0.42.0 peft==0.8.2 trl==0.7.10 accelerate==0.27.1 datasets==2.17.0 transformers==4.38.0


##  Repo structure

Gemma-LoRA-FineTuning/
├── .env
├── requirements.txt
├── finetune_gemma.ipynb
├── README.md
└── 

2. Environment Variables
Create a .env file:

HF_TOKEN=your_hf_token_here

 Example

Input:
Quote: A woman is like a tea bag;

Output:
Quote: A woman is like a tea bag; you never know how strong she is until she's in hot water. Author: Eleanor Roosevelt


📝 Dataset
Dataset: Abirate/english_quotes

