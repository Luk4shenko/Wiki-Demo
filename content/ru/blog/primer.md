---
title: "Пример Markdown документа"
date: 2023-07-14
draft: false
---

# Пример Markdown документа

## Введение

Это пример документа, демонстрирующего различные элементы и возможности Markdown.

## Форматирование текста

Вы можете использовать **жирный**, *курсив*, или ***жирный курсив***. Также доступно ~~зачеркивание~~.

## Заголовки

# Заголовок 1
## Заголовок 2
### Заголовок 3
#### Заголовок 4
##### Заголовок 5
###### Заголовок 6

## Списки

### Маркированный список
- Элемент 1
- Элемент 2
  - Подэлемент 2.1
  - Подэлемент 2.2
- Элемент 3

### Нумерованный список
1. Первый элемент
2. Второй элемент
3. Третий элемент

## Ссылки и изображения

[Ссылка на OpenAI](https://www.openai.com)

![Логотип Markdown](https://markdown-here.com/img/icon256.png)

## Цитаты

> Это пример цитаты. Она может содержать несколько строк и даже включать другие элементы Markdown.

## Код

Встроенный `код` выглядит так.

Блок кода:

```python
def hello_world():
    print("Hello, World!")

hello_world()
```

## Горизонтальная линия

---

## Таблицы

| Заголовок 1 | Заголовок 2 | Заголовок 3 |
|-------------|-------------|-------------|
| Ячейка 1,1  | Ячейка 1,2  | Ячейка 1,3  |
| Ячейка 2,1  | Ячейка 2,2  | Ячейка 2,3  |

## Задачи

- [x] Выполненная задача
- [ ] Невыполненная задача
- [ ] Еще одна задача

## Сноски

Это предложение содержит сноску[^1].

[^1]: Это текст сноски.

## Определения

Markdown
: Легковесный язык разметки с синтаксисом форматирования обычного текста.

HTML
: Стандартизированный язык разметки для создания веб-страниц.

## Эмодзи

Вы можете использовать эмодзи в Markdown! :smile: :heart: :thumbsup:

## KaTeX

KaTeX shortcode let you render math typesetting in markdown document. See [KaTeX](https://katex.org/)

### Example

<div class="book-columns flex flex-wrap">
  <div class="flex-even markdown-inner">

```latex
{{</* katex display=true class="optional" >}}
f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
{{< /katex */>}}
```

  </div>
  <div class="flex-even markdown-inner">

{{< katex display=true class="optional" >}}
f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
{{< /katex >}}

  </div>
</div>

### Display Mode Example

Here is some inline example: {{< katex >}}\pi(x){{< /katex >}}, rendered in the same line. And below is `display` example, having `display: block`
{{< katex display=true >}}
f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
{{< /katex >}}
Text continues here.

## Диаграммы (используя Mermaid в Hugo)

Hugo поддерживает диаграммы Mermaid из коробки. Вот несколько примеров:

## Примеры диаграмм Mermaid для Hugo

### Блок-схема

{{< mermaid >}}
graph TD
    A[Начало] --> B{Есть ли проблема?}
    B -- Да --> C[Решить проблему]
    C --> D[Конец]
    B -- Нет --> D
{{< /mermaid >}}

### Диаграмма последовательности

{{< mermaid >}}
sequenceDiagram
    participant Пользователь
    participant Сервер
    participant База данных
    Пользователь->>Сервер: Запрос данных
    Сервер->>База данных: Запрос к БД
    База данных-->>Сервер: Результат запроса
    Сервер-->>Пользователь: Ответ с данными
{{< /mermaid >}}

### Диаграмма состояний

{{< mermaid >}}
stateDiagram-v2
    [*] --> Ожидание
    Ожидание --> Обработка: Получен запрос
    Обработка --> Отправка: Данные готовы
    Отправка --> Ожидание: Ответ отправлен
    Отправка --> [*]: Ошибка
{{< /mermaid >}}

### Диаграмма Ганта

{{< mermaid >}}
gantt
    title Проект по разработке
    dateFormat  YYYY-MM-DD
    section Планирование
    Анализ требований      :a1, 2023-01-01, 7d
    Проектирование         :a2, after a1, 5d
    section Разработка
    Кодирование            :a3, after a2, 15d
    Тестирование           :a4, after a3, 7d
    section Развертывание
    Подготовка             :a5, after a4, 2d
    Запуск                 :a6, after a5, 1d
{{< /mermaid >}}

## Уведомления или заметки

### Example

{{< hint info >}}
**Markdown content**  
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
{{< /hint >}}

{{< hint warning >}}
**Markdown content**  
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
{{< /hint >}}

{{< hint danger >}}
**Markdown content**  
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
{{< /hint >}}

## Заключение

Это лишь некоторые из возможностей Markdown. Помните, что поддержка некоторых расширенных функций (таких как формулы, диаграммы или уведомления) может зависеть от конкретной реализации Markdown-рендерера.