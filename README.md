# LLM_Classification_Finetuning
Large language models (LLMs) are rapidly entering our lives, but ensuring their responses resonate with users is critical for successful interaction. This competition presents a unique opportunity to tackle this challenge with real-world data and help us bridge the gap between LLM capability and human preference.

I utilized a large dataset collected from Chatbot Arena, where users chat with two anonymous LLMs and choose the answer they prefer. The task in this competition is to predict which response a human would prefer in these head-to-head battles.

This challenge aligns with the concept of "reward models" or "preference models" in reinforcement learning from human feedback (RLHF). Previous research has identified limitations in directly prompting an existing LLM for preference predictions. These limitations often stem from biases such as favoring responses presented first (position bias), being overly verbose (verbosity bias), or exhibiting self-promotion (self-enhancement bias).

This competition challenge is to predict which responses a human would prefer in a head-to-head battle between chatbots powered by large language models (LLMs).

https://www.kaggle.com/competitions/llm-classification-finetuning

# Evaluation
Submissions are evaluated on the log loss between the predicted probabilities and the ground truth values (with "eps=auto").

# Submission File
For each id in the test set, you must predict the probability for each target class. The file should contain a header and have the following format:

 | id       | winner_model_a | winner_model_b | winner_tie |
|----------|----------------|----------------|------------|
| 136060   | 0.33           | 0.33           | 0.33       |
| 211333   | 0.33           | 0.33           | 0.33       |
| 1233961  | 0.33           | 0.33           | 0.33       |
| etc      | ...            | ...            | ...        |

# Requirements
  - Python 3.9 or Python 3.10

# Installation
  1. Download this repository or clone it using `git clone https://github.com/0Kan0/LLM_Classification_Finetuning`.
  2. Access the downloaded folder. (Optional: Create a virtual environment and activate it).
  3. Install the required packages by running `pip install -r requirements.txt`.
  4. Run the notebook.
