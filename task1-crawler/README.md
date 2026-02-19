## WebCrawler

Веб-краулер для скачивания страниц с сайта ria.ru.

### Требования

- **Java 23**
- **Maven**

### Запуск


```bash
cd task1-crawler
mvn exec:java
```

### Результат

После выполнения в папке `downloaded_pages/` будут сохранены HTML-файлы, а в `index.txt` — индекс соответствий номеров файлов и URL.
