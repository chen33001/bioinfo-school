---
name: Lessons
description: "Use when doing bioinformatics related tasks in Agents"
---

# Week 1 — What an LLM actually is

## Reading

- Jin et al., *[GeneGPT: Augmenting Large Language Models with Domain Tools for Improved Access to Biomedical Information](https://academic.oup.com/bioinformatics/article/40/2/btae075/7606338)*

### notes from paper

- GeneGPT achieves the best performance on eight GeneTuring tasks with an average score of 0.83, which is remarkably higher than the previous SOTA (0.44 by New Bing). 
- the author teaches GeneGPT to use NCBI Web APIs through in-context learning with a carefully designed prompt
- using 9 GeneTuring tasks that are related to NCBI resources to evaluate the proposed GeneGPT model
- tasks are classified into four modules (1) Nomenclature (2) Genomics location (3) Functional analysis (4) Sequence alignment
- comparing GeneGPT with GPT-2, GPT-3, and chatGPT
- GeneGPT largely surpasses various LLMs on GeneTuring
- characterize GeneGPT by studying four research questions (RQ): (1) (2) (3) (4)


## Video

- Andrej Karpathy, *[Deep Dive into LLMs like ChatGPT](https://www.youtube.com/watch?v=7xTGNNLPyMI)* (3h31m, Feb 2025).

### notes from Video

- Fineweb pipeline start with raw website text (one sequence) from hugging face
- tradeoff between the number of symbols and the length of the sequence
- tokenizer visualize the how GPT 4-o turn 0,1 symbol into 1300 symbols
- reproduction of GPT 2
- different parameter (weights) would make a huge difference (currently not really, many small models can still have good performance)
- base model = internet document simulator
- pretraining(long) -> base model -> post-training: supervised finetuning(short)
- hallucination -> mitigation (1) new training example (2) tool use (ex: RAG)
- SFT model post-training (reinforcement learning)
- Reinforcement learning from human feedback (allow people to attribute to performance of model without doing difficult tasks)
- RLHF can improve the model, but not necessary guarantee
- multimodal (text to audio, images, video, natural conversations)
- tasks -> agents