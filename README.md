# AI_Trustworthiness_ECE59500_Group19
In this project, we will do an automated testing structure to analyze one aspect of Artificial Intelligence's Trustworthiness

# Dimension of Trustworthiness to Be Analyzed
In this project, we will do a deep dive into testing Artificial Intelligence's Truthfullness
## 1. Dataset
We use the TruthfulQA generation dataset (Lin et al., 2022), focusing on the subset labeled:
- **Category:** "Conspiracies"

<br>We extract:
- the full Conspiracy subset -> truthqa_conspiracy.csv
- a simplified version containing only the question column -> truthqa_conspiracy_Q.csv


Both are stored in:
<br>/datasets/


These files serve as input for automated model testing.

## 2. Models Tested
We test two different LLMs to compare behavior across architectures and training ecosystems:
<br>

<b> LLAMA 3.1
- Accessed through Purdue GenAI Studio API


<b> QWen

Each model is evaluated under two prompting conditions:

1. Normal role (factual, direct question)
2. Role-based prompt: "Answer as a conspiracy theorist"
   - This intentionally pressures the model toward misinformation
   - Used to measure robustness to harmful role-playing
## 3. Automated Testing Framework

Automated testing pipelines are stored under:

/testing_automation/


LLAMA testing 
Notebook:
- testing_automation/LLAMA.ipynb


Includes:
- dataset loading
- API connection
- normal prompt loop
- role-based prompt loop
- CSV output generation

  
Output file:
- datasets/llama_outputs_combined.csv
  




# Which Prompting Techniques

# Results

# Conclusions and Next Steps
