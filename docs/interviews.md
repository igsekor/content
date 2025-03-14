# Рубрика «На собеседовании»

Техническое собеседование — сложный процесс. Мы хотим помочь успешно пройти это испытание, лучше разобраться в веб-платформе, придать уверенности и позитива. В наших статьях есть специальная рубрика, в которой контрибьюторы и могут задавать вопросы и давать ответы на них.

## Как задать вопрос

Проверьте, нет ли такого вопроса на Доке. Загляните в [задачи](https://github.com/doka-guide/content/issues?q=is%3Aopen+is%3Aissue+label%3Aсобеседование), чтобы ознакомиться со списком вопросов, на которые ещё нет ответов на Доке.

Если ваш вопрос ещё не был задан, [создайте задачу](https://github.com/doka-guide/content/issues/new?assignees=&labels=&template=3_empty.md&title=).

## Как написать ответ

1. Найдите в директории _interviews_ папку с вопросом. В подпапке _answers_ находятся ответы на вопрос. Каждый ответ лежит в своей папке, название которой совпадает [с никнеймом автора ответа](#ваша-подпись). Создайте свою папку для ответа.

2. Каждый ответ — это отдельный Markdown-файл. Создайте файл _index.md_ внутри своей папки и напишите свой вариант.

Мета ответа может оставаться пустой, в этом случае ответ будет отображаться во всех материалах, в которых будет появляться и вопрос. Если потребуется показывать ответ только в части материалов, то список папок материалов должен быть в одном из списков `excluded` (для исключения) или `included` (для включения). Пример:

```markdown
---
excluded:
  - html/bdo
---

## Подзаголовок в ответе на поставленный вопрос

Можно использовать всё богатство формата Mardown и для ответа

```

Главный фокус этой рубрики — корректный и ёмкий ответ на собеседовании. Удалось ли подать свой ответ каким-то интересным образом? Знаете как лучше ответить? Эта рубрика для вас!

💡 Если ваш ответ — скорее подсказка, добавьте его в раздел «Подсказки» в теле статьи.

💡 Если вы хотите просто дополнить материал какой-то информацией, которой там не хватает для успешного собеседования — тоже добавьте её в саму статью.

Если вы впервые контрибьютите в Доку, создайте ещё собственную директорию в папке _people_ репозитория _content_ и расскажите о себе [по примеру в документации](people.md). Это нужно, чтобы к вашему совету сгенерировался корректный заголовок с вашим именем.

## Как написать вопрос и ответ

1. Создать папку с уникальным именем в папке _interviews_.

2. Создать Markdown-файл _index.md_.

3. В мете вопроса в поле `related` нужно перечислить пути в материалам Доки, в которых должен появится ваш вопрос.

Пример:

```markdown
---
related:
  - html/bdo
  - css/flexbox-guide
  - css/position
---

Вопрос, который можно услышать на собеседовании.

Если потребуется, то пояснение вопроса, для которых можно использовать все возможности формата Markdown.
```

4. Создать ответ по инструкции из [предыдущего пункта](#как-написать-ответ).

У вас должна получится следующая структура папок:

```markdown
interviews
└── some-question
    ├── answers
    │   └── doka-dog
    │       └── index.md
    └── index.md
```

### Структура ответа

Структура ответа проста. Как правило, это абзац или несколько. Можно дополнять текст примерами кода и [демками](demos/index.md).

### Стиль ответа

В ответах можно и нужно говорить от себя: «я считаю», «я делаю так», «я советую», но можно использовать и безличную форму подачи. Ваше имя все равно будет в заголовке.

Чтобы быть на волне Доки, почитайте наше [руководство по стилю](styleguide.md).

Спасибо за ваш вклад!

## Ваша подпись

Ваш ответ на вопрос можно подписать. Для этого воспользуйтесь [инструкцией по созданию профиля пользователя](people.md).

Если у вас уже есть профиль, проверьте, что название папки в директории `/people/` совпадает с названием в директории `/interviews/**/answers/`. Если видите своё имя из профиля, то всё отлично, если нет, переименуйте папку в `/interviews/**/answers/`.
