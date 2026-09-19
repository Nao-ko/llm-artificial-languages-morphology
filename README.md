# Study 1: Artificial-language morphology

This repository contains the article and the data behind it: an experiment testing whether Qwen2.5-1.5B-Instruct can infer the morphological structure of five artificial languages, with and without English translations.

## Contents

- `article.tex`: the full article (LaTeX source).
- `acl.sty`: the LaTeX style file required to compile `article.tex`.
- `figures/`: the figure used in the article.
- `data/`: the artificial-language datasets and the scored comparison tables (with vs. without English).
- `raw_outputs/`: the raw model annotations, before scoring.
- `details/`: the per-item scoring details behind the summary tables in the article.

## Data

- `dataset_with_english.csv` / `dataset_without_english.csv`: the five artificial languages, generated from shared meanings.
- `language_key.json`: the ground truth for each artificial language (intended type and key grammatical markers), used to score the model's output.
- `comparison_with_english.csv` / `comparison_without_english.csv`: scores per language and condition (marker, function, feature, overall).
- `with_vs_without_english_summary.csv` / `with_vs_without_english_paired_comparison.csv`: the paired comparison between the two conditions.
- `raw_outputs/`: the model's raw text output for each language, before any scoring was applied.
- `details/`: the item-level scoring behind each summary score.

The ground truth is included here so that the scoring can be checked and reproduced.
