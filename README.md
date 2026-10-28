# Machine Learning CA2 — Case Studies 3 & 4

## Included projects

### Case Study 3: E-Commerce Customer Segmentation
- UCI Online Retail transaction dataset
- RFM feature engineering: Recency, Frequency, Monetary
- K-Means with silhouette-based K selection
- DBSCAN and noise-point analysis
- PCA and t-SNE visualization
- Cluster profiles, heuristic marketing personas, and recommendations

### Case Study 4: Sentiment Analysis on Product Reviews
- Amazon reviews loaded with HuggingFace Datasets
- Three sentiment classes: negative, neutral, positive
- Fine-tuned DistilBERT (a compact BERT-family transformer) via HuggingFace Trainer
- LSTM baseline implemented in PyTorch
- Accuracy, macro precision/recall/F1, classification reports, confusion matrices
- Transfer-learning and deployment constraints

## Setup

Recommended Python 3.10 or 3.11. Use a virtual environment:

```bash
python -m venv .venv
# Windows
.venv\\Scripts\\activate
# macOS/Linux
source .venv/bin/activate

python -m pip install --upgrade pip
pip install -r requirements.txt
```

Open both notebooks in Jupyter, VS Code, or Google Colab. Run cells from top to bottom.

## Data
- Case Study 3 downloads the UCI Online Retail archive if `data/Online Retail.xlsx` is missing. If download fails, obtain the dataset from the UCI Machine Learning Repository and save it under that filename.
- Case Study 4 downloads the English `amazon_reviews_multi` dataset and pretrained model weights from HuggingFace; internet access is needed on first run.
- Raw data and model outputs are excluded from Git to avoid oversized repositories.

## Reproducibility and honest reporting
- Metrics and cluster profiles are computed during execution; this repository does not contain fabricated scores.
- K-Means tests K=2 through K=6 and selects the best silhouette score.
- DBSCAN `eps=0.7` and `min_samples=10` are starting values; discuss the clusters/noise produced by your actual run.
- t-SNE uses a reproducible sample of up to 3,000 customers.
- Sentiment mapping: stars 1–2 negative, 3 neutral, 4–5 positive.
- Sample sizes and epochs can be increased if hardware permits.
- Record actual results and conclusions after running the notebooks.

## Before submission
1. Run both notebooks top to bottom.
2. Save notebook outputs so plots, metrics, and tables are visible.
3. Add your own short conclusion using actual output.
4. Ensure you can explain RFM, K-Means, DBSCAN, PCA, t-SNE, BERT fine-tuning, LSTM, macro-F1, and deployment trade-offs.
5. Never upload passwords, API keys, or personal credentials.

Suggested GitHub repository name: `ML-CA2-Case-Studies`.
