После перевода текста в в токены с помощью Word Embeddings или TF-IDF и т.п. нужно это предобработать:
Приведение к нижнему регистру
Удаление пунктуации
Удаление стоп-слов
Лемматизация и стемминг
Удаление чисел
Удаление HTML-тегов
Удаление шума

ТОКЕНЫ - ТЕКСТОВЫЕ ЕДИНИЦЫ

## Tokenization

Libs: NLTK, TextBlob, spaCy, Gensim, PyTorch, Keras

- Sentence tokenization

\["Hello, world!"]

- Word tokenization

\["Hello,", "world!"]

``` python
import nltk
from nltk.tokenize import word_tokenize, senq_tokenize
text = "Hello, world!"
print(word_tokenize(text))
```

Treebank: don't -> \["do", "n't"]
Tweet: smiles отдельно
`"Если у человека в нике какой-то флаг в твиттере - он дегенерат." by albert`

MWET: 'Hunger', 'Games' -> add() -> "Hunger_Games"

Стемминг удаляет extra символы от значения слова по типу суффиксов, окончаний.
seen -> see

Лемматизация приводит к каноническому виду, а не удаляет последние значения.
drove -> drive

Ngrams: Скользящее окно по словам. Например, для кластеризации у больших данных будет работать медленно

Stop-words: удаляет ненужные слова по типу "is, are, a, the, of". В русском могут быть предлоги и т.п.

Regular expressions . \w \d \s \W \D \S \[abc] \[^abc] \[a-g]
import re

# BoW (Bag of words)

Создает словарь в виде:
- Ключ - слово
- Значение -  количество этого слова в тексте

Пример:
``` python
"Я люблю и папу, и маму"
```

Создаем словарь с словами:
``` python
["Я", "люблю", "и", "папу", "маму"]
```

где BoW-вектор это
``` python
[1, 1, 2, 1, 1]
```

Очень простой и быстро обучается, но не учитывает: 
- порядок слов, 
- значение (пес и собака разные индексы, хотя близкие по значению), 
- может быть много нулей, что создает проблему разряженностью (sparse). Способен занимать много места, работать медленно без оптимизаций, очень большая размерность.

Предобрабатывают обычно так:
- Удаление спец символов, разметки
- Приведение к нижнему регистру
- Удаление стоп слов: "и", "в", "на", "это"

## Measures of Similarity

Scale sensitive and not sensitive
- distance-based: euclidean, manhattan, minkowski, chebyshev
- feature-based
- probabilities

Levenshtein distance
Damerau-Lebenshtein distance
Lee distance
Hamming distance
Jaro distance
Jaro-Winkler distance

Levenshtein:
- substitute, insert, delete
- you can modify "weights" of each action
- useful for autocorrection, misspelling and etc.

Sensitive: cosine sim, square euclidian (L2 norm), Dot product (работает с проекцкией)

Processing images:
- "factual" лоб в лоб
- "semantic" содержание











