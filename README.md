# Егор Хоробрых

**Data Scientist (Computer Vision / NLP / Time Series)**

Самара | Удалённо

Telegram: [@ac3err](https://t.me/ac3err) | egorhorobryh@gmail.com | +7 (909) 717-55-71

---

## О себе

Data Scientist с 7 месяцами коммерческого опыта в компьютерном зрении (детекция, классификация, регрессия). Реализовал полный цикл ML-проектов: от валидации и обучения до оптимизации инференса и упаковки в CLI/Desktop-приложения. Работал с CV (сегментация, детекция, OCR), NLP (fine-tuning и квантизация T5, RAG) и временными рядами. Финалист хакатона Т1-Импульс, 2 место на CodeGym 2.0.

---

## Навыки

- **Языки:** Python, SQL, C++ (базовый)
- **Deep Learning:** PyTorch, Hugging Face Transformers, TensorFlow
- **Computer Vision:** OpenCV, YOLO, Albumentations, сегментация (U-Net, U-Net++, DeepLabV3+), OCR (PyTesseract)
- **NLP / LLM:** fine-tuning T5, квантизация, суммаризация, RAG, hybrid retrieval (BM25 + Dense), reranking
- **Classic ML:** scikit-learn, XGBoost, CatBoost, LightGBM, кросс-валидация, feature engineering
- **Time Series:** TCN, LSTM, Transformer, VAE, GARCH-симуляции
- **Data:** pandas, NumPy, SciPy, Matplotlib, Seaborn, Plotly, PySpark
- **Инструменты:** Git, Linux, Jupyter, PyYAML, Qdrant, Docker

---

## Опыт работы

### ИНТЕГРА-С, Самара | ML Engineer
*Апрель 2026 - настоящее время*

- Исследовал и разработал алгоритмы детекции драк на основе оценки поз (`YOLO-pose`+`GNN/RNN+GNN/Transformer+GNN`) достигнув `meanPrecision@100frames = 0.912`
- Разработал и реализовал программы для полуавтоматической разметки данных (`yolo/sam2`, `yolo-pose`)
- Разработал и обучил модели детекции и классификации изображений

---

## Проекты

### SmartNotes | `Python`, `PyTorch`, `Hugging Face`, `mT5-small`
[github/egortens1a/SmartNotes](https://github.com/egortens1a/SmartNotes)

Десктопное приложение для локальной суммаризации текстов без внешних API.

- Дообучил multilingual T5-small и применил квантизацию (`ONNX`), ускорив обработку текста до 1000 слов **с >30 с до 7 с** на CPU
- Качество суммаризации: **BERTScore F1 = 0.85**
- Датасет **Gazeta** - это русскоязычный набор данных для задач автоматического суммаризации текстов и доступный на платформе [Hugging Face](https://huggingface.co/datasets/IlyaGusev/gazeta)

### Fire Segmentation | `PyTorch`, `Albumentations`, `OpenCV`
[github/egortens1a/fire-segmentation](https://github.com/egortens1a/fire-segmentation)

Сегментация пламени на изображениях.

- Обучил и сравнил U-Net, U-Net++ и DeepLabV3+ с бэкбонами ResNet и EfficientNet
- Лучший результат: `U-Net++ с энкодером EfficientNet-B3, val IoU = 0.85]`
- Разработал CLI-инструмент с конфигурацией через YAML: обработка изображений произвольного разрешения, выгрузка бинарных и вероятностных масок, наложение оверлеев

### tsprep  *(в разработке)* | `PyTorch`, `scikit-learn`
[github/egortens1a/tsprep](https://github.com/egortens1a/tsprep)

Исследование нейросетевых методов сжатия и анализа экономических временных рядов.

- Сравнил классические модели и DL-архитектуры (TCN, LSTM, Transformer, VAE), включая гибрид TCN + Self-Attention
- Написал генератор синтетических рядов (стохастический тренд, многомасштабная сезонность, GARCH-волатильность, смены режимов)
- Оценка через Downstream Linear Probe, Silhouette-скор латентных режимов, $F1$ детекции аномалий, $MSE$/$MAE$/$R^2$

### Berserk AI *(в разработке)* | `Qdrant`, `RAG`, `Cross-Encoder`
[github/KlimentiiFrolov/Berserk_ai](https://github.com/KlimentiiFrolov/Berserk_ai)

RAG-модуль для бота-консультанта по ККИ Берсерк.

- Спроектировал hybrid retrieval (Dense + BM25) в Qdrant с RRF-fusion и cross-encoder reranking для точной работы с доменными терминами

### Хакатон Т1-Импульс 2024 | `PyTorch`, `YOLO`, `PyTesseract`, `OpenCV`

Финалист, трек Распознавание рукописного текста на банковских документах. Пайплайн: YOLO для поиска текстовых областей -> предобработка -> OCR.

---

## Образование

**Самарский университет им. С.П. Королева**
Бакалавриат, Прикладная математика и информатика, 2022 - 2027

---

## Курсы

- Deep Learning (CV & NLP), Deep Learning School, ФПМИ МФТИ, `2024-2025`
- ИИ и машинное обучение (программа по переквалификации: ML-engineer), Цифровая кафедра Самарского университета
- ML-тренировки (сезоны 2-4), Яндекс, 2024-2025
- Базовый курс по анализу данных, Т-Банк, 2025
[Таблица полным списком пройденных курсов](https://docs.google.com/spreadsheets/d/1fIziZeTsGjRot8MULBzJ-4ffXFzrT5jj/edit?usp=sharing&ouid=114270286365945063019&rtpof=true&sd=true)

---

## Достижения

- 2 место, CodeGym 2.0 Самара 2025
- Финалист хакатона Самара Т1-Холдинг 2024
- III разряд по спортивному программированию