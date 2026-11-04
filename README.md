# Егор Хоробрых

**ML Engineer**

Самара | Удалённо

Telegram: [@ac3err](https://t.me/ac3err) | egorhorobryh@gmail.com | +7 (909) 717-55-71


## О себе

ML Engineer с коммерческим опытом в компьютерном зрении - детекции событий на видео, классификации изображений и полуавтоматической разметке. Работал на разных этапах ML-проектов, от подготовки данных и обучения моделей до оценки качества, оптимизации инференса и разработки прикладных инструментов. Также есть опыт в сегментации изображений, суммаризации текстов, поиске для RAG и прогнозировании временных рядов.


## Навыки

- **Языки:** Python, SQL, C++ (базовый)
- **Deep Learning:** PyTorch, Hugging Face Transformers
- **Computer Vision:** OpenCV, YOLO, Albumentations, сегментация (U-Net, U-Net++, DeepLabV3+), OCR (PyTesseract)
- **NLP / LLM:** fine-tuning T5, квантизация, суммаризация, RAG, hybrid retrieval (BM25 + Dense), reranking
- **Classic ML:** scikit-learn, XGBoost, CatBoost, LightGBM, кросс-валидация, feature engineering
- **Time Series:** TCN, LSTM, Transformer, VAE, GARCH-симуляции
- **Data:** pandas, NumPy, SciPy, Matplotlib, Seaborn, Plotly
- **Инструменты:** Git, Linux, Jupyter, Qdrant, Docker


## Опыт работы

### ИНТЕГРА-С, Самара | ML Engineer
*Апрель 2026 - настоящее время*

- Исследовал и сравнил подходы к детекции опасных событий на видео на основе оценки поз человека (pose estimation + графовые и последовательностные нейросети), достигнув **Precision > 0.9**
- Разработал инструменты полуавтоматической разметки видеоданных и изображений на базе YOLO и SAM2: модели генерируют рамки, маски и скелеты, которые разметчик проверяет и корректирует
- Обучал и дообучал модели детекции и классификации изображений (PyTorch, YOLO) на собственных датасетах: подготовка данных, аугментации, подбор гиперпараметров, оценка качества на валидации

## Проекты

### SmartNotes | `Python`, `PyTorch`, `Hugging Face`, `mT5-small`
[github/egortens1a/SmartNotes](https://github.com/egortens1a/SmartNotes)

Десктопное приложение для локальной суммаризации текстов без внешних API.

- Дообучил multilingual T5-small и применил квантизацию (`ONNX`), ускорив обработку текста до 1000 слов **с >30 с до 7 с** на CPU
- Качество суммаризации: **BERTScore F1 = 0.85**
- Обучение на русскоязычном датасете [Gazeta](https://huggingface.co/datasets/IlyaGusev/gazeta) для задачи автоматической суммаризации текстов

### Fire Segmentation | `PyTorch`, `Albumentations`, `OpenCV`
[github/egortens1a/fire-segmentation](https://github.com/egortens1a/fire-segmentation)

Сегментация пламени на изображениях.

- Обучил и сравнил U-Net, U-Net++ и DeepLabV3+ с бэкбонами ResNet и EfficientNet
- Лучший результат: `U-Net++` с энкодером `EfficientNet-B3`, **val IoU = 0.85**
- Разработал CLI-инструмент с конфигурацией через YAML: обработка изображений произвольного разрешения, выгрузка бинарных и вероятностных масок, наложение оверлеев

### tsprep  *(в разработке)* | `PyTorch`, `scikit-learn`
[github/egortens1a/economic-timeseries-preprocessing](https://github.com/egortens1a/economic-timeseries-preprocessing)

Исследование нейросетевых эмбеддингов для прогнозирования экономических временных рядов.

- Настроил прогноз преобразованного ряда AAPL и BTC на 5 шагов вперёд с помощью Ridge на эмбеддингах TCN, LSTM и Transformer
- Добавил хронологическое разбиение, сравнение с Ridge на исходных окнах и PCA-признаках, а также парные bootstrap-интервалы для разницы ошибок
- Написал генератор синтетических рядов с трендом, сезонностью, GARCH-волатильностью и сменами режимов

### Berserk AI *(в разработке)* | `Qdrant`, `RAG`, `Cross-Encoder`
[github/KlimentiiFrolov/Berserk_ai](https://github.com/KlimentiiFrolov/Berserk_ai)

RAG-модуль для бота-консультанта по ККИ Берсерк. Участвую в роли RAG/ML-разработчика, отвечаю за систему поиска и оценку качества системы.

- Спроектировал гибридный поиск в Qdrant. Объединил результаты BM25 и dense-поиска через RRF и добавил переранжирование с помощью cross-encoder

### Хакатон Т1-Импульс 2024 | `PyTorch`, `YOLO`, `PyTesseract`, `OpenCV`

Финалист, трек Распознавание рукописного текста на банковских документах. Пайплайн: YOLO для поиска текстовых областей -> предобработка -> OCR.


## Образование

**Самарский университет им. С.П. Королева**
Бакалавриат, Прикладная математика и информатика, 2022 - 2027


## Курсы

- Deep Learning (CV & NLP), Deep Learning School, ФПМИ МФТИ, `2024-2025`
- ИИ и машинное обучение (программа по переквалификации: ML-engineer), Цифровая кафедра Самарского университета
- ML-тренировки (сезоны 2-4), Яндекс, 2024-2025
- Базовый курс по анализу данных, Т-Банк, 2025

[Таблица полным списком пройденных курсов](https://docs.google.com/spreadsheets/d/1fIziZeTsGjRot8MULBzJ-4ffXFzrT5jj/edit?usp=sharing&ouid=114270286365945063019&rtpof=true&sd=true)


## Достижения

- 2 место, CodeGym 2.0 Самара 2025
- Финалист хакатона Самара Т1-Холдинг 2024
