## Boolean Search

Построение инвертированного индекса и булев поиск по лемматизированным документам.

### Требования

- **Java 23**
- **Maven**
- Результат работы Task2: папка `task2-tokenizer/processed_tokens/lemmatized` с лемматизированными файлами
- Кодировка ввода и вывода UTF8 в консоли

### Запуск

**1. Сборка проекта:**

```bash
cd task3-boolean-search
mvn compile
```

**2. Построение инвертированного индекса:**

```bash
cd task3-boolean-search
mvn exec:java -Dexec.mainClass="main.java.InvertedIndexBuilder"
```

**3. Интерактивный булев поиск:**

```bash
cd task3-boolean-search
mvn exec:java -Dexec.mainClass="main.java.BooleanSearch"
```

Поддерживаются операторы `and`, `or`, `not` и скобки. Примеры запросов: `слово1 and слово2`, `слово1 or слово2`, `not слово`, `(слово1 or слово2) and слово3`.

### Результат

После построения индекса в корне проекта создаётся файл `inverted_index.txt`. При запуске BooleanSearch доступен интерактивный ввод запросов (для выхода введите `exit`).
