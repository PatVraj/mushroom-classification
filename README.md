# Mushroom Classification Data Science

## Overview
A comprehensive analytical deep-dive into mushroom classification, leveraging advanced data science techniques to classify poisonous vs. edible mushrooms. This project focuses on evaluating whether a mushroom's toxicity can be determined based on easily identifiable human features or basic physical properties.

[View the Data Science Project Report](./mushroom-ds.pdf)

[View the Project Presentation](./Adv%20Data%20Science_%20Final%20Project.pptx)

## Architecture / Tech Stack
- **Language**: Python
- **Libraries**: Scikit-Learn, Pandas, NumPy, Matplotlib
- **Methodology**: K-Means Clustering, Gaussian Mixture Models (GMM), Feature Extraction

```mermaid
flowchart TD
    A[Mushroom Dataset (61k+ rows)] --> B[Data Preprocessing & Cleaning]
    B --> C[K-Means Clustering]
    B --> D[Gaussian Mixture Models]
    C & D --> E[Interpretability / Feature Importance]
    E --> F[Classification Results (Edible vs Poisonous)]
```

## Local Setup Instructions
```bash
git clone https://github.com/PatVraj/mushroom-classification.git
cd mushroom-classification
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook Notebook/shrooms.ipynb
```

## Key Results / Metrics
- Processed a dataset of 61,069 mushrooms across 173 species with 20 distinct attributes.
- Explored GMM across various values of `k` (1 to 11) using the elbow method to discover hidden distributions, finding an optimal 68% representation purity at 5 clusters.
- Utilized K-Means clustering (initially with numerical features like cap diameter, stem height, and stem width) to map complex patterns to toxicity rates.
- Investigated the inclusion of categorical features via custom distance metrics (Jaccard similarity).

## Data Provenance & Licensing
- Sourced from Kaggle (Mushroom Classification Edible or Poisonous).

## Collaborators
- Vraj Patel, Jasdeep Singh, Nikhil Chakka
