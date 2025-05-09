# Prompt Engineering with GPT-2 and BERTScore

## Overview

This project demonstrates prompt engineering techniques using the GPT-2 language model to generate motivational content, with quality evaluation performed using BERTScore. The implementation follows a structured approach to:

- Generate diverse motivational content using different prompt styles  
- Compare outputs against human-written references  
- Evaluate semantic similarity using BERTScore metrics  
- Analyze which prompt strategies produce the most human-like results  

---

## Features

- Five distinct prompt styles:
  - Direct instruction
  - Scenario-based
  - Persona-based
  - Keyword-based
  - Conversational approach  
- Automated quality evaluation using **BERTScore F1** metric  
- Reproducible results with seed setting and parameter control  
- Comprehensive outputs including:
  - Generated texts
  - Evaluation scores
  - Submission checklist  

---

## Requirements

To run this project, you'll need:

- Python 3.7+
- PyTorch
- HuggingFace Transformers
- BERTScore
- Pandas

Install all dependencies with:

```bash
pip install torch transformers bert-score pandas
```

---

## Project Structure

The implementation is provided in two formats:

### 1. Jupyter Notebook (`Prompt_Engineering_GPT2_BERTScore.ipynb`)
- Interactive environment for experimentation  
- Step-by-step execution with visual outputs  
- Markdown explanations between code cells  

### 2. Python Script (`prompt_engineering.py`)
- Command-line executable version  
- Automated workflow from start to finish  
- Results saved to CSV file  

---

## Usage

### Jupyter Notebook

1. Open the notebook in Jupyter
2. Run cells sequentially
3. View outputs and analysis after each section
4. Customize prompts in **Part 2** as needed

### Python Script

```bash
python prompt_engineering.py
```

**Outputs will be:**
- Printed to the console
- Saved to `prompt_engineering_results.csv`

---

## Methodology

- **Model Loading**: GPT-2 base model from HuggingFace Transformers  
- **Prompt Engineering**: Five distinct prompt strategies  
- **Text Generation**:
  - 3 variations per prompt
  - Sampling parameters:
    - `temperature`: 0.7
    - `top_k`: 50
    - `top_p`: 0.95  
- **Evaluation**: BERTScore F1 metric comparing to human-written references  
- **Analysis**: Results table comparing effectiveness of each prompt style  

---

## Results Interpretation

The output includes:

- Generated texts for each prompt type  
- BERTScore F1 values (range 0–1, higher is better)  
- Comparison table showing which prompt styles performed best  
- Complete submission checklist  

---

## Customization

You can experiment with the following parameters:

- `temperature` (controls randomness of outputs)  
- `top_k` and `top_p` (affect output diversity)  
- Prompt structure and wording  
- Human reference texts for evaluation  

---

## License

This project is licensed under the **MIT License**.

---

## References

- Radford, A. et al. (2019). *Language Models are Unsupervised Multitask Learners*.  
- HuggingFace Transformers: https://huggingface.co/transformers/  
- BERTScore: https://github.com/Tiiiger/bert_score  
