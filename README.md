# Requirements

Лучше всего, если до изучения этого у вас есть базовые познания в линейной алгебре, возможно в математическом анализе и в статистике/теории вероятности.
# Outline:
Регрессия (Regression) 
Линейная регрессия (1) 
Полиномиальная регрессия (1) 
Ridge + Lasso + Elastic Net (2) 
Байесовская регрессия (3) 
Регрессия по деревьям (2)

Классификация (Classification) 
Наивный байес (Naive Bayes) (1) 
Gaussian Naive Bayes (1) 
Метод k-ближайших соседей (KNN) (1) 
Дерево решений классификатор и регрессия (Decision Tree Classifier and Regression) (1) 
Случайный лес классификатор и регрессия (Random Forest Classifier and Regression) (2) 
Метод опорных векторов (SVM) (2) 
Max-margin classification (2) 
Лагранжиан SVM (Lagrangian SVM) (3) 
QDA (Quadratic Discriminant Analysis) (2) 
Градиентный бустинг (GBDT) (2)

Кластеризация (Clustering) 
K-Means (1) 
K-Means ++ (2) 
Иерархическая кластеризация (Hierarchical Clustering) (2) 
DBSCAN (2) 
Mean-Shift (2) 
Silhouette Clustering (3) 
Affinity Propagation (3) 
OPTICS (3)

Ансамблевые методы (Ensemble Methods) 
AdaBoost (2) 
Стеккинг (Stacking) (3) 
XGBoost (2) 
LightGBM (2) 
CatBoost (2) 
Voting (2) 
Blending (3)

Снижение размерности (Dimensionality Reduction) 
PCA (1) 
SVD (2) 
t-SNE (2) 
UMAP (3)

Перцептрон (Perceptron) 
Perceptron (1) 
Adaline (1)

Глубокое обучение (Deep Learning)

Нейронные сети 
Сверточные нейронные сети (CNN) (2) 
Рекуррентные нейронные сети (RNN) (LSTM, GRU) (2) 
Двунаправленные RNN (Bidirectional RNN) (3) 
Полносвязные нейронные сети (FNN) (2) 
Автоэнкодеры (Autoencoder) (3) 
Вариационные автоэнкодеры (Variational Autoencoder) (3) 
Остаточные сети (Residual Networks) (3) 
Сеть СИАМ (Siamese Network) (3) 
Памятные сети (Memory Networks) (3) 
Машина Больцмана (Boltzmann Machine) (3) 
Сеть Хопфилда (Hopfield Networks) (3) 
Глубокая сеть убеждений (Deep Belief Network) (3) 
GANs (Generative Adversarial Networks) (3) 
Reinforcement Learning Networks (DQN) (3) 
Graph Neural Networks (GNN) (3)

Трансформеры и последовательности 
Трансформеры (Encoder, Decoder, Attention) (3) 
Seq2Seq (3) 
Встраивания (Embeddings) (2) 
BERT и варианты (3) 
Attention-only models (3)

Эволюционные архитектуры 
Evolving Architectures NEAT (3) 
Genetic Algorithms for NN (3) Neuroevolution (3)

Углубление

Обработка естественного языка (NLP - Natural Language Processing) Bag of Words (BoW) (1) TF-IDF (Term Frequency-Inverse Document Frequency) (1) Word Embeddings (Word2Vec, GloVe) (2) N-grams (2) Latent Dirichlet Allocation (LDA) (2) Named Entity Recognition (NER) с CRF (Conditional Random Fields) (3) Sentiment Analysis с Naive Bayes (2)

Компьютерное зрение (CV - Computer Vision) Haar Cascades (1) Viola-Jones Algorithm (1) Edge Detection (Canny, Sobel) (1) HOG (Histogram of Oriented Gradients) (2) SIFT (Scale-Invariant Feature Transform) (2) SURF (Speeded-Up Robust Features) (2)

Усиленное обучение (RL - Reinforcement Learning) Q-Learning (2) SARSA (2) Deep Q-Networks (DQN) (3) Policy Gradient Methods (3) Actor-Critic Methods (3)

## Сбор данных
	Источник данных (1)
    Сбор данных (1)
    Валидация с самого начала (1)
	Синтетические данные (2)

## Explanatory data analysis
    Обзор данных (1)
    Описательная статистика (1)
    Визуализация распределений (1)
    Поиск выбросов (1)
    Анализ зависимостей (2)
    Проверка пропусков (1)
    Анализ временных рядов (3)
    Feature importance (3)
    Анализ сезонности (3)

## Data wrangling
    Очистка пропусков (1)
    Удаление выбросов (1)
    Преобразование типов (1)
    Удаление дубликатов (1)
    Интеграция данных (2)
    Фильтрация по релевантности (2)
    Генерация новых признаков из внешних данных (3)
    Работа с большими данными (Bigdata) (3)

## Feature engineering
    Математические преобразования (1)
    Кодирование категориальных данных (1)
    Бинаризация (2)
    Извлечение из дат (2)
    Агрегация (2)
    Нормализация/масштабирование (1)
    Полиномиальные признаки (3)
    Для текстовых признаков можно добавить эмбеддинги (3)
    Feature Selection (2)

## Data spliting
    Деление данных (Возможно еще на валидационный набор) (1)
    Балансировка классов (2)
    Stratifying (2)

## Model Training
    Выбор алгоритма (1)
    Обучение модели (1)
    Кросс-валидация (2)
    Добавление baseline-модель (2)
    Оптимизация модели для ускорения инференса (квантизация, sparsification) (3)
    Автоматизация выбора модели (3)

## Model Evaluation
    Оценка на тестовой выборке (1)
    Использование метрик (1)
    Анализ ошибок (2)
    Анализ важности признаков (2)
    Confidence intervals для метрик (3)
    Анализ ошибок на основе explainability tools ((SHAP, LIME и т.п.)) (3)

## Model Tuning
    Подбор гиперпараметров ИЛИ (2)
    Автоматизированный подбор гиперпараметров (3)
    Улучшение алгоритма (2)

## Model Serialization
    Сохранение модели (1)
    Сохранение препроцессинга (2)

## Integration
    Интеграция в код (API + Инференс) (1)
    Пайплайн предобработки (1)
    Логика приложения (Human Ai interaction design) (2)
    Обработка исключений (2)
    Версионирование моделей (3)
    Кэширование предсказаний (3)

## Testing
    Unit Testing (отдельных компонентов) (2)
    Integration Testing (весь пайплайн вход->предсказание) (1)
    Stress Testing (под нагрузкой) (3)
    A/B-тестирование (3)

## Containerization
    Создание DockerFile (1)
    Сборка контейнера (1)
    Docker Compose (2)

## Deployment
    Локальный деплой (1)
    Облачный деплой (2)
    CI/CD настройка (2)
    Скейлинг (3)
    Edge deployment (3)

## Monitoring & Maintenance
    Логирование (Время запросов, ошибки и т.п.) (1)
    Мониторинг качества (метрики) (2)
    Обновление модели (Переобучение модели на новых данных) (2)
    Обратная связь (Сбор данных для улучшения) (3)
    Алерты (При падении метрик) (3)
    Мониторинг данных (Data Drift и Concept Drift Detection) (3)
    Отслеживание аномалий в данных (3)
    Автоматический откат модели при падении метрик (3)
