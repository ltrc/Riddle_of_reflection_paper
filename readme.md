# The Riddle of Reflection: Evaluating Reasoning and Self-Awareness in Multilingual LLMs Using Indian Riddles

This is the official repository for the paper **"The Riddle of Reflection: Evaluating Reasoning and Self-Awareness in Multilingual LLMs Using Indian Riddles."** 

This repository contains the curated datasets and prompt templates used to test the reasoning capabilities and self-awareness of Large Language Models (LLMs) across seven major Indian languages: Bengali, Gujarati, Hindi, Kannada, Malayalam, Tamil, and Telugu.

## 🗂️ Repository Structure

Based on our three-phase methodology, the repository is organized as follows:

* **`data/`**: Contains the core multilingual riddle datasets.
  * **`96_riddles/`**: `.tsv` files containing the 96 curated traditional original riddles and their answers for each of the 7 Indian languages.
  * **`context_reconstructed_riddles/`**: `.json` files containing the high-quality, human-curated context-reconstructed variants used for our context-reconstructed few-shot prompting.
  * **`semantic_similar_riddles/`**: Datasets organized for the semantic similarity few-shot prompting experiments.
* **`prompts/`**: Contains the exact prompt templates used for evaluating the models.
  * Language-specific directories (e.g., `bengali`, `gujarati`, etc.) housing the 0-shot, random few-shot, semantic few-shot, and context-reconstructed few-shot prompts.
  * **`yes_or_no_prompts/`**: The single-token output prompts used for the Phase 3 Self-Evaluation task.


## 📊 About the Task
Solving riddles requires complex multi-step commonsense reasoning, metaphorical interpretation, and deep cultural knowledge. This project evaluates models not only on their ability to generate the correct answer (**Riddle-Solving**) but also on their ability to correctly identify if their own generated answer was right or wrong (**Self-Awareness**).

**Key Finding:** Our evaluation reveals a crucial "Self-Awareness Paradox" in modern LLMs—top-performing models (like Gemini 2.5 Pro) are highly overconfident and fail to recognize their own mistakes, whereas lower-performing models exhibit substantially better self-awareness.



## 📝 Citation
If you use this dataset or code in your research, please consider citing our paper:
```text
@misc{m2025riddlereflectionevaluatingreasoning,
      title={The Riddle of Reflection: Evaluating Reasoning and Self-Awareness in Multilingual LLMs using Indian Riddles}, 
      author={Abhinav P M and Ojasva Saxena and Oswald C and Parameswari Krishnamurthy},
      year={2025},
      eprint={2511.00960},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2511.00960}, 
}