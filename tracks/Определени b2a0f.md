# Определение версии opensource-ПО по git-репозиторию

Created: February 9, 2022 5:26 PM
Mentor: yorxx
Tags: хакатон

## Описание:

Многие компании используют открытое программное обеспечение в своей работе. Нам, как пентестерам, важно определять его версию, однако не везде она указана явно: нет указания ни в теле ответа, ни в скриптах, нет и файлов README и CHANGELOG. Тем не менее, возможность определить версию имеется: можно сравнивать публичные ресурсы (html, js, css) в репозитории с теми, которые получаешь с сервера. Таким образом можно получить коммит или диапазон коммитов установленной версии, их теги и, чаще всего, версию ПО. Напишите утилиту, позволяющую определить версию opensource-ПО по git-репозиторию.

## Что мы хотим:

Консольная утилита на языке Python или go. На вход утилита принимает URI целевого сайта, путь к git-репозиторию и указание целевой папки в нем, разрешения файлов, которые можно получить и сравнить. На выходе утилита отдает идентификатор коммита или диапазона коммитов, которым соответствует установленная версия, их тэги.

## Критерии оценки:

Корректность работы, алгоритм выбора файлов для сравнения, скорость и удобство работы.