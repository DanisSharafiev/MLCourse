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







