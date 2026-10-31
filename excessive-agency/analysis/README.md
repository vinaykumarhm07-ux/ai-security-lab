# Analysis utilities

Run `python analyze.py --gpt PATH_TO_GPT_OSS_JSONL --qwen PATH_TO_QWEN_JSONL --out sanitized_results.jsonl`.

The script reports API coverage, removes duplicate Qwen prompt rows while preferring successful responses, and emits metadata-only sanitized results. It never writes raw model response text. The qualitative labels for Qwen prompts 147–172 are manually assigned and should be independently reviewed before being treated as benchmark scores.
