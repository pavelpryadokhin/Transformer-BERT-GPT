# Transformer-BERT-GPT
Работа с моделями в области NLP, изучение их архитектуры.

## Файл Transformer
Взята классическая архитектура трансформера (статья [Attention is All You Need](https://arxiv.org/pdf/1706.03762))
* Был построен трансформер для задачи question answering.
* Использован датасет с [HuggingFace](https://huggingface.co/datasets/Den4ikAI/russian_dialogues).
* Был написан собственный доработанный токенизатор (CustomTokenizer).

## Файл BERT
Взята предобученная [BERT-модель](https://huggingface.co/google-bert/bert-base-uncased) и доработана для того, чтобы она могла отвечать на вопросы, основанные на контексте.
* Был использован набор данных SQuAD
* Получены удовлетворительные результаты на легких вопросах

  
