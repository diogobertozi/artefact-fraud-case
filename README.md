# Artefact fraud detection case

Diogo Bertozi's submission for the Artefact data science case. The notebook ranks transactions for fraud review.

## Run the notebook

1. Place the recruiter-provided `transacoes_historico_2025.csv` and `transacoes_jan2026.csv` beside `fraud_case.ipynb`.
2. Install Python 3 with Jupyter, pandas, NumPy, scikit-learn and Matplotlib.
3. Open `fraud_case.ipynb` and run all cells. The notebook writes the January classifications to `submission/january_2026_predictions.csv`.

The public repository contains the analysis code. The supplied transaction data and row-level predictions are delivered through the application.

## Evaluation

The notebook trains on January–September 2025, selects the model and threshold on October–November, and evaluates on December. Histogram gradient boosting achieved 60.65% precision, 59.06% recall, and 0.5914 average precision on December. Initial exploratory profiling inspected December labels.

The final refit on all 2025 data flagged 2,348 of 44,451 January 2026 transactions. January labels were unavailable for evaluation.
