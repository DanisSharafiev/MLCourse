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








