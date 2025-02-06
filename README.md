# Transformer-BERT-GPT
Работа с моделями в области NLP, изучение их архитектуры.

## Файл Transformer
Взята классическая архитектура трансформера (статья [Attention is All You Need](https://arxiv.org/pdf/1706.03762))
* Был построен трансформер для задачи question answering.
* В качестве основы был использован датасет, доступный на [HuggingFace](https://huggingface.co/datasets/Den4ikAI/russian_dialogues).
* Для повышения эффективности работы был разработан собственный улучшенный токенизатор, получивший название CustomTokenizer.

## Файл BERT
Взята предобученная [BERT-модель](https://huggingface.co/google-bert/bert-base-uncased) и доработана для того, чтобы она могла отвечать на вопросы, основанные на контексте.
* Был использован набор данных SQuAD
* На простых вопросах результаты оказались удовлетворительными.

## Файл GPT
Мы использовали [предварительно обученную модель GPT2](https://huggingface.co/ai-forever/rugpt3small_based_on_gpt2) и обучили её создавать заголовки к русскоязычным новостным статьям.
* Для обучения модели был использован [датасет от Lenta.ru](https://www.kaggle.com/datasets/yutkin/corpus-of-russian-news-articles-from-lenta).
* Для более качественного обучения были выбраны статьи за последние три года.
* Для генерации заголовков была настроена функция model.generate.
