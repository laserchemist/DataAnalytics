# Teaching notebook: Corporate venturing text analysis

Open `sws_cv_text_analysis_teaching.ipynb` (latest version; `cv_text_analysis_teaching.ipynb` is the first draft) with the `data/` folder next to it. It runs in about 10 seconds with no API key.

| File | Contents |
|---|---|
| `data/passages.csv` | 19 short passages (Alphabet, Microsoft, Merck): 10-K excerpts and scraped web text, including deliberate keyword "traps" |
| `data/definitions.csv` | The 15 framework dimensions (programs, activities, objectives) from `framework_v2` |
| `data/cached_llm_responses.json` | Saved answers to the notebook's LLM prompt, so it works offline |
| `data/pipeline_scores.csv` | Full-pipeline emphasis scores for 6 companies (`outputs_v2`) |
| `data/pipeline_score_cards.json` | Score, top quote, rationale and 5-pass samples per dimension for GOOGL and MRK |

Requirements: `pip install pandas matplotlib scikit-learn` (add `anthropic` for live calls with `USE_API = True`).
