# llama-1b-dialogsum-finetuned
## Overview
This repository includes:
- Fine-tuning a pre-trained small language model (Llama 1b) using LoRA and PEFT.
- Running training with specified configurations.
- Evaluating the model both qualitatively and quantitatively (using ROUGE metric).
- Saving the fine-tuned model and uploading it to Hugging Face.

# Sample output
For sample outputs please refer to the image attached

# Absolute percentage improvement of PEFT MODEL over ORIGINAL MODEL

rouge1: 5.07%
  PEFT model has a 5.07% higher ROUGE-1 score than the original model.
  This means that in terms of unigram overlap, the PEFT model captures more of the important words.

rouge2: 2.23%
  The ROUGE-2 score is 2.23% higher for the PEFT model.
  This means that the PEFT model is slightly better at capturing common bigrams.

rougeL: 4.81%
  The PEFT model shows a 4.81% improvement in the ROUGE-L score.
  ROUGE-L measures the longest common subsequence, so this shows the PEFT model maintains a better overall sequence similarity.

rougeLsum: 5.88%
  With a 5.88% higher ROUGE-Lsum score, the PEFT model shows improved performance in summarization tasks.
  This score reflects how well the generated summary aligns with the reference summary in terms of structure and content.

Overall based on Rouge and manual tests, PEFT models seems to perform a bit better than the base model

The deployed model can be found at: https://huggingface.co/Amna1917e81729/llama-1b-dialogsum-finetuned
