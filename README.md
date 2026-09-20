# Pavel Alekseev

**Junior ML / LLM Engineer · HSE MSc in Machine Learning (with honours)**

I build ML and LLM applications end to end: data, training, evaluation and a service around the model. My background combines machine learning and finance: MSc in Machine Learning at HSE and MSc in Financial Economics at HSE ICEF. Some of that work is public, including a retrieval benchmark and a fine-tuned embedding model for Russian law, both on Hugging Face. Open to remote roles.

## Projects

| Project | What it is |
|---|---|
| [Anime Video Super-Resolution](https://github.com/alekseevpavel04/Anime-Video-Super-Resolution-via-GAN-Upscaling) | **Master's thesis:** ×2 anime video upscaling; RRDBNet GAN, Swin2SR and ESRT compared under three degradation pipelines, TensorRT video inference |
| [ru-law-retrieval](https://github.com/alekseevpavel04/ru-law-retrieval) | Open retrieval benchmark over 3,786 articles of six Russian codes in MTEB format, plus a fine-tuned embedder. 19 minutes of training on one RTX 3070 moves `multilingual-e5-small` from 0.802 to 0.859 nDCG@10, matching `multilingual-e5-large` at 4.8x the parameters and 6.8x the CPU latency. [Model](https://huggingface.co/alekseevpavel04/multilingual-e5-small-ru-law) and [dataset](https://huggingface.co/datasets/alekseevpavel04/ru-law-retrieval) on Hugging Face |
| [tk-rf-rag](https://github.com/alekseevpavel04/tk-rf-rag) | RAG Q&A over the Russian Labor Code, now running the fine-tuned embedder above, Qdrant / FAISS behind one interface, FastAPI, answers cite articles and refuse when the context has no answer; 30-question eval with Hit@k / MRR, LLM-as-a-judge faithfulness and a chunk-size experiment. Swapping in the fine-tuned embedder moved MRR@5 on a 716-question hard set from 0.688 to 0.793 |
| [vk_claude_bot](https://github.com/alekseevpavel04/vk_claude_bot) | Claude Agent SDK assistant in VK chats with a tool whitelist, SSRF protection and a resource-capped Docker deployment |
| [co2_detector](https://github.com/alekseevpavel04/co2_detector) | Battery-powered CO₂ / temperature / humidity monitor built end to end: ESP32-S3 + SCD41 + e-Paper, power-optimised C++ firmware (PlatformIO) with native unit tests, 3D-printed OpenSCAD case |
| [todaysmenu](https://github.com/alekseevpavel04/todaysmenu) | Telegram recipe bot: Qwen2.5 query rewriting, allrecipes.com scraping, streaming, LLM-as-a-judge benchmark |
| [ASR with PyTorch](https://github.com/alekseevpavel04/Automatic-Speech-Recognition-ASR-with-PyTorch) | DeepSpeech2-style speech recognition on LibriSpeech with KenLM beam search; WER 24.4 on test-other |
| [ai_text_detector](https://github.com/alekseevpavel04/ai_text_detector) | FastAPI service and Telegram bot for paragraph-level AI-text detection with a pretrained DeBERTa classifier |
| [respondo](https://github.com/alekseevpavel04/respondo) | Prototype browser extension that suggests chat replies via a FastAPI backend and Gemini |

## Open-source contributions

Merged:

- MLflow: [#25260](https://github.com/mlflow/mlflow/pull/25260) Flush the `SpanBatcher` from the trace flush paths so UC-table spans are exported
- MLflow: [#25514](https://github.com/mlflow/mlflow/pull/25514) Reject unsupported `env_manager` values when building a model container

More PRs under review in Prefect, ZenML and Feast.

## Stack

Python · PyTorch · Hugging Face Transformers · sentence-transformers · embedding fine-tuning (contrastive learning, knowledge distillation) · RAG (Qdrant, FAISS) · MTEB · scikit-learn · FastAPI · Docker · Hydra · Weights & Biases · TensorRT · LLM APIs (Claude Agent SDK, Gemini)

## Contacts

- Telegram: [@pavel0420](https://t.me/pavel0420)
- Email: alekceevpavel@mail.ru
