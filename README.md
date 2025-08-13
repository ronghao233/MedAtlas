# MedAtlas
MedAtlas: Evaluating LLMs for Multi-Round, Multi-Task Medical Reasoning Across Diverse Imaging Modalities and Clinical Text

Below is a portion of the dataset. The final version will be made public later.

## Dataset Structure

Each data sample includes the following fields:

- `chat_id`: Unique identifier for each case
- `round_id`: Dialogue turn identifier
- `text_prompt`: Full text input, including patient history and question content
- `instruction`: Final instruction given to the model before answering
- `images`: List of image URLs used for diagnostic reference
- `assistant`: The model’s answer content, formatted with question-answer pairs
- `correct_option_letters`: List of correct choices for each question (e.g., ["A", "C", "D"])
- `model_name`: The name of the model generating the response (e.g., "gpt-4o")

