## TfIdfCalculator

Калькулятор TF-IDF для токенов и лемм. Вычисляет веса терминов на основе частоты в документе и обратной частоты документа в коллекции.

### Требования

- **Java 23**
- **Maven**
- Данные из **task2-tokenizer**: папки `processed_tokens/tokens` и `processed_tokens/lemmatized`

### Запуск

```bash
cd task4-tf-idf
mvn compile
mvn exec:java "-Dexec.mainClass=main.java.TfIdfCalculator"
```

### Результат

После выполнения в папке `tf-idf-output/tokens/` будут сохранены файлы с TF-IDF для токенов, в `tf-idf-output/lemmas/` — для лемм. Каждая строка содержит: `термин IDF TF-IDF`.
