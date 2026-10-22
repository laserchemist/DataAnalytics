# Data for sentiment_vader_teaching.ipynb

| File | What it is |
|---|---|
| `tweets_raw.csv` | The original 200 tweets, unchanged except that the `user_id` column was removed. VADER 3.3.2 columns: negative, neutral, positive, compound. |
| `tweets_clean.csv` | 176 unique tweets. Exact duplicates removed (`n_copies` = how many there were), HTML codes such as `&amp;` decoded, IDs kept as text. Hand-made flags: `multi_line`, `is_spam`, `language` (English vs. non-English/mixed, approximate), `mentions_peeple`. |
| `excerpts.csv` | The 22 teaching excerpts: W1-W2 (handout worked examples), H1-H8 (handout), E1-E12 (notebook only), with the trap each one tests and a suggested label toward Facebook. |
| `transformer_scores.csv` | Not included. Created when you run the optional RoBERTa cell once with `USE_TRANSFORMER = True`. |

Always read IDs as text: `pd.read_csv(..., dtype={"tweet_id": str})`.
