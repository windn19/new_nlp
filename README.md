# NLP

Проект создан в учебных целях с использованием предобученной модели для перевода текста с английского языка на русский
и передачи его по API. Для создания API использовался фреймворк FastAPI и UviCorn.

## Запуск

1. Для запуска необходимо выполнить установку зависимостей из файла requirements.txt

```bash
pip install -r requirements.txt
```

2. Запуск веб приложения совершается через команду run

```bash
uvicorn main:app
```

3. В проекте есть две точки доступа: index и predict

- при передаче GET запроса по адресу /index - возвратится json - с текстом "Hello World!!!"
- при передаче POST запроса по адресу /predict/ c передачей в теле запроса параметра "text", в котором передается текст
  для перевода
- по GET запросу по адресу /docs - будет выведена автоматически сгенерированная документация с указанием точек доступа
  и параметров для отправки запросов, а также форма получаемых ответов.

Выполнил Дмитрий Носков.
