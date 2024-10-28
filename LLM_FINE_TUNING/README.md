# Notebooks for Finetuning LLMs on your Data.

We currently have two different methods for finetuning here:
1. GPT-4o-mini
2. Llama-3.1-8b

### GPT-4o-mini

- Fine-tuning an OpenAI doesn't explicitly require GPU access as the Fine-tuning happen on their cloud.

### Llama-3.1-8b

- If you are going to Fine-tune Llama 3.1 8b, doing so on Google colab or some other jupyter environment which provide GPU access is a must. 
- Here, I have personally used Google colab with T4 GPU.
- You can create your own dataset and modify the templates according to your needs.

## Note:

I haven't provided the Dataset for LLama 3.1 Fine-tuning notebook hence you'll have to create your own but if you're not sure how to start, here is a structure of dataset on which i fine-tuned my model, `dataset.json`:

```json
[
    {
        "case_title": "...",
        "Instruction": "...",
        "input": "...",
        "response": "..."
    },
    {
        "case_title": "...",
        "Instruction": "...",
        "input": "...",
        "response": "..."
    },
]
```