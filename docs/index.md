# Welcome to MkDocs

## Съдържание на плъгини

### hotlink to repository

```yml
repo_name: Github
repo_url: https://github.com/dragomir-d/unit-docs/
edit_uri: 'docs/'
```

### page revision date

Показва последната дата на редакция на страницата, визуализира се най-отдолу на всяка страница.

За да сработи трябва да има настроен [hotlink to repository](#hotlink-to-repository) в `mkdocs.yml`.

Инсталация:

```
pip install mkdocs-git-revision-date-plugin
```

Добавяме git-revision-date в `mkdocs.yml`:

```yml
plugins:
    - search
    - git-revision-date
```

Добавката `search` е активирана по подразбиране, но в съчетание с git-revision-date ако тя не бъде подадена ще бъде деактивирана.

### PDF export

Супер удобен бутон за PDF export директно на машината. Трябва инсталация на [Weasyprint](https://doc.courtbouillon.org/weasyprint/latest/first_steps.html#windows), това е инструмент, който преобразува html в PDF файлове.

Като инсталираме weasyprint, следва да инсталираме плъгина в mkdocs:

```
pip install mkdocs-pdf-export-plugin
```

Добавяме в `mkdocs.yml`:

```
plugins:
    - pdf-export:
        combined: true
```

`combined: true` ще гарантира, че целият сайт ще бъде експортнат в един pdf файл.

## Image or diagram

![image](test.png)