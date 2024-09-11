# TineyReview - Comparative Analysis of Small Language Models (SLMs) with Preprocessing Techniques

## Overview

This project focuses on optimizing Small Language Models (SLMs) by implementing preprocessing techniques and constructing efficient datasets. By refining data to its essential elements, we aim to improve grammatical accuracy, diversity, and reasoning in text generation. The project demonstrates how SLMs can achieve comparable results to larger models with reduced computational and memory costs.

## Key Features

- **Customized GPT-Neo Model:** Implemented a modified architecture with embedding layers and transformer blocks, capable of generating coherent sentences after a short training period.
- **Preprocessing Pipelines:** Developed various preprocessing techniques to optimize datasets, including the data with specific Part-Of-Speech Structure only, or filtering out uncommon words.
- **Dataset Construction:** Created datasets from Amazon Book Reviews with different preprocessing strategies, each improving model performance in specific areas.
- **Performance Evaluation:** Used both GPT-3.5 and GPT-4 for automated and manual evaluations of the model’s grammar, creativity, and consistency.

## Project Structure

- **Model Training Scripts:** Code to train the SLM models can be found in `Training.ipynb`.
- **Evaluation Scripts:** Manual evaluation scripts for analyzing model performance are in `ManuallyEvaluation.ipynb`.
- **Datasets:** Preprocessed datasets used for training and testing are available on Hugging Face under the names `TinyReviews_raw`, `books_raw`, and `kindle`.

## Installation and Setup

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-repository/slm-analysis.git
    cd slm-analysis
    ```

2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Download datasets from Hugging Face:**
   - [TinyReviews with Raw Data](https://huggingface.co/ChunB1/TinyReviews_raw)
   - [TinyReviews with Common Verbs only](https://huggingface.co/ChunB1/TinyReviews_common)
   - [TinyReviews with Noun, Verb, and Adj](https://huggingface.co/ChunB1/TinyReviews_adj)
   - [TinyReviews with Noun, Verb, Adj, and Adv](https://huggingface.co/ChunB1/TinyReviews_adv)

4. **Run model training:**
   Open `Training.ipynb` in Jupyter and run the cells to train the models with different preprocessing strategies.

## How to Use

1. **Training Models:**
   You can train the models using the provided scripts. Ensure you have access to a GPU for faster training, as the models are optimized for V100 GPUs.

2. **Evaluating Models:**
   The models can be evaluated using GPT-3.5 or GPT-4. Follow the instructions in `ManuallyEvaluation.ipynb` to generate performance metrics.

3. **Dataset Preprocessing:**
   The datasets have been preprocessed to improve model efficiency. Refer to the dataset section for detailed preprocessing steps, including vocabulary size reduction and sentence structure optimization.

## Results

The results indicate that SLMs trained on carefully curated datasets can generate outputs comparable to larger models with a fraction of the computational cost. Key improvements in grammar, consistency, and creativity were observed, especially with the dataset containing a balanced mix of verbs, nouns, adjectives, and adverbs.

## Contributors

- **Alan Yang:** Designed project flow and conducted qualitative analysis.
- **Xu Michael:** Constructed datasets, trained models, and handled quantitative evaluations.
- **Massoud Mahsa:** Contributed to the design, conducted research, and wrote the report.
