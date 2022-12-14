# **Инструкция по работе с Git**

# Что такое Git?

Git - это набор консольных утилит, которые отслеживают и фиксируют изменения в файлах. С его помощью можно сравнивать, анализировать, редактировать и возвращаться к последнему сохранению.

# Cоздание локального репозитория

Чтобы открыть конкретную папку или файл используем команду:

    git init

# Проверка состояние репозитория

Чтобы проверить состояние репозитория используем команду:

    git status
    
# Добавление файла для отслеживания

Чтобы добавить файл для отслеживания используем команду:

    git add

# Сохранение измененений 

Чтобы сохранить изменения в файле используйте команду:

    git commit

откроется текстовый редактор в котором вы сможете оставить комментарий к сохранению, чтобы потом удобно ориентироваться в истории изменений.

Чтобы оставить комментарий прямо из командной строки вместо тектового редактора используйте команду:

    git commit -m

# Просмотр истории коммитов

После того, как вы создали несколько коммитов, вероятно вам понадобится возможность посмотреть что было сделано — историю коммитов. Одним из основных и наиболее мощных инструментов для этого является команда:

    git log

# Переключение между коммитами

Чтобы переключиться между последними сохранениями или вызвать нужный коммит, используйте команду:

    git cheackout

Чтобы вернуться к самой актульной версии файла используйте команду:

    git cheackout master

# Просмотр изменений

Чтобы просмотреть изменения и проанализировать выходные данные используйте команду:

    git diff

# Добавление изображений

![logo](git.jpg)

# Ветвления

Используя ветвление, Вы отклоняетесь от основной линии разработки и продолжаете работу независимо от неё, не вмешиваясь в основную линию. Это нужно для удобства написания файла, внесения изменений и их отслеживания разными пользователями.

Чтобы создать новую ветвь используйте команду:

    git branch <name branch>

Чтобы переключаться между ветками, переходить на определенную ветвь и вносить там изменения, используйте команду:

    git checkout <branch name>

# Cоздание слияния

Когда требуется добавить изменения из одной ветки в другую (произвести слияние), используйте команду:

    git merge <branch name>

и программа добавит изменения из указанной ветки в текущую.

 Обычно после слияние веток одну из них удаляют, это можно сделать при помощи команды:

    git branch -d <branch name>

# Просмотр истории коммитов

Для просмотра истории сохранений мы используем команду git log, но в таком случае программа покажет нам коммиты только на текущей ветке, чтобы посмотреть коммиты на всех ветках, используйте команду:

    git log --all

А чтобы увидеть краткий список коммитов добавьте:

    git log --all --oneline

Для визуализации ветвления используйте команду:

    git log --all --oneline --graph

## Удаленные репозитории

Удаленные репозитории нужны для...
