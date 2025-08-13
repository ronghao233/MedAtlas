# MedAtlas
MedAtlas: Evaluating LLMs for Multi-Round, Multi-Task Medical Reasoning Across Diverse Imaging Modalities and Clinical Text

Below is a portion of the dataset. The final version will be made public later.
**Dataset URL**: [https://huggingface.co/datasets/ronghao233/auntqa](https://huggingface.co/datasets/ronghao233/auntqa)
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

## Example

```json
{
  "chat_id": "chat_1",
  "round_id": "round_1",
  "text_prompt": "History: A 46-year-old man presented with ...",
  "instruction": "You are a doctor. Please answer each question...",
  "images": [
    "https://my.auntminnie.com/image1.jpg",
    "https://my.auntminnie.com/image2.jpg"
  ],
  "assistant": "Question 1\nCorrect: A\nExplanation: ...",
  "correct_option_letters": ["A", "C", "D"],
  "model_name": "gpt-4o"
}
