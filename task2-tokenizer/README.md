## Tokenizer

Скрипт для обработки HTML‑страниц из проекта `task1-crawler`: извлекает текст, токенизирует его, удаляет стоп‑слова и строит лемматизированные списки токенов.

### Требования

- **Python 3.10.10**
- Установленные зависимости из `requirements.txt`:

  ```bash
  pip install -r requirements.txt
  ```

### Запуск

1. Убедитесь, что в соседнем проекте `task1-crawler` уже скачаны страницы и есть папка `task1-crawler/downloaded_pages`.
2. Перейдите в папку `task2-tokenizer`:

   ```bash
   cd task2-tokenizer
   ```

3. (Рекомендуется) создать и активировать виртуальное окружение Python.
4. Установите зависимости:

   ```bash
   pip install -r requirements.txt
   ```

5. Запустите скрипт:

   ```bash
   python tokenizer.py
   ```

Во время первого запуска `nltk` автоматически скачает необходимые ресурсы (`punkt`, `stopwords`).

### Результат

После выполнения в папке `processed_tokens` появятся две подпапки:

- `processed_tokens/tokens` — файлы `tokens_имя_страницы.html.txt` с очищенными токенами;
- `processed_tokens/lemmatized` — файлы `lemmatized_имя_страницы.html.txt` с леммами и соответствующими им формами слов.

