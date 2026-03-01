## SearchSystem

Поисковая система на основе векторной модели. Ранжирует документы по косинусному сходству TF-IDF лемм запроса и документов.

### Требования

- **Python 3.10.10**
- Установленные зависимости из `requirements.txt`
- Данные из **task1-crawler**: `index.txt`
- Данные из **task4-tf-idf**: `tf-idf-output/lemmas/`

### Запуск

Установка зависимостей:

```bash
cd task5-search
pip install -r requirements.txt
```

Консольный режим:

```bash
cd task5-search
python main.py
```

Веб-интерфейс:

```bash
cd task5_search
python run_demo.py
```

### Результат

Возвращает топ-10 наиболее релевантных URL по запросу, отсортированных по степени сходства.
