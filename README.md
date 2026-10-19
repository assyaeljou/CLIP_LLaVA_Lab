# CLIP & LLaVA — Vision-Language Models Lab

A hands-on lab exploring **CLIP** and **LLaVA-OneVision** using Python, PyTorch, and Hugging Face Transformers.

The project covers image classification, image retrieval, visual question answering (VQA), and hallucination testing.

## Models

| Model | Purpose |
|---|---|
| CLIP | Image-text similarity, zero-shot classification, and image retrieval |
| LLaVA-OneVision | Image description and visual question answering |

## Lab Contents

- **CLIP:** Image and text embeddings, classification, and prompt engineering.
- **Image Retrieval:** Search images using text descriptions.
- **LLaVA:** Answer questions about images and test hallucinations.
- **Model Comparison:** Compare CLIP and LLaVA.
- **Mini-Project:** Build a simple multimodal image assistant.

## Key Results

- CLIP classified 10 cat and dog images correctly (100% accuracy).
- Prompt wording affected CLIP's similarity scores.
- CLIP retrieved images using text descriptions.
- LLaVA correctly identified the absence of a bicycle in a test image.
- VQA results were saved in `vqa_results.csv`.

*Note: The experiments use small datasets, so the results are indicative only.*

## Project Structure

```text
CLIP_LLaVA_Lab/
├── LAB_CLIP_LLaVA_Full_Lab_Statement.ipynb
├── clip_image_database.pt
├── vqa_results.csv
├── images/
├── requirements.txt
├── .gitignore
└── README.md
```

## Installation

**Requirements:** Python 3.11+ and Git.

### 1. Clone the repository

```bash
git clone https://github.com/assyaeljou/CLIP_LLaVA_Lab.git
cd CLIP_LLaVA_Lab
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

## Usage

Start Jupyter Notebook:

```bash
jupyter notebook LAB_CLIP_LLaVA_Full_Lab_Statement.ipynb
```

Run the notebook cells from top to bottom.

**Important:**
- Keep the input images inside the `images/` folder.
- Run Exercise 7 before using the image retrieval bonus.
- Exercise 11 generates `vqa_results.csv`.
- The models download automatically on the first run. An internet connection is required.
- A GPU is recommended for faster LLaVA inference.

## Troubleshooting

| Problem | Solution |
|---|---|
| Missing Python packages | Run `pip install -r requirements.txt`. |
| Jupyter cannot find packages | Select the correct Python virtual environment as the notebook kernel. |
| Images not found | Run Jupyter from the project directory. |
| LLaVA runs slowly | Use a GPU or Google Colab. |

## Limitations

- Small datasets and limited evaluation.
- CLIP results depend on the candidate labels and prompt wording.
- LLaVA may produce incorrect answers or hallucinate details.

## References

- Radford et al. (2021), *Learning Transferable Visual Models From Natural Language Supervision*.
- Liu et al. (2023), *Visual Instruction Tuning*.
- Li et al. (2024), *LLaVA-OneVision: Easy Visual Task Transfer*.
- [Hugging Face Transformers Documentation](https://huggingface.co/docs/transformers)

## Author

**Assya El Jounaidi**

GitHub: [@assyaeljou](https://github.com/assyaeljou)