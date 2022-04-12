# Руководство по работе с Git

## Основные команды

* Для инициализации репозитория используют команду *git init*
* Для добавления файла - *git add*
* Для создания коммита (сохранения) - *git commit -m ""*
* Для выяснения статуса файла - *git status*
* Для вызова истории изменений - *git log*

## Работа с ветками

1. Для обзора существующих веток используют команду ***git branch***.
2. Для создания новой ветки используют команду ***git branch branch_name***, где ***branch_name*** - название создаваемой ветки. 
3. Для переключения между ветками - ***git checkout branch_name***. Эту же команду используют для переключения между коммитами, но вместо ***branch_name*** необходимо указать первые 4 символа коммита.
4. Для того, чтобы создать новую ветку и сразу переключиться на нее используют команду ***git checkout -b branch_name***.
5. Для слияния 2 веток используют команду ***git merge branch_name***, но для этого необходимо находиться на той ветке, куда будет происходить слияние.
6. Для удаления ненужной ветки используют команду ***git branch -d branch_name***. 
7. Для графического изображения веток - ***git log --graph***.

# Конфликты при слиянии

Конфликты при слиянии могут возникать в том случае, если 2 ветки противоречат друг другу. Или 1 ветка опережает другую. Например, если в 1 ветке исправилии или удалили текст, который содержит главная ветка, а потом попытались их объединить.