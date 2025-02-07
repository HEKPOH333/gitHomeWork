# Инструкция по работе с Git, а также описание команд.
## Базовые команды 
* ***Git init*** - Команда инициализации локального репозитория.
* ***Git status*** - Команда получения текущего стостояния git.
* ***Git cgeckout*** - Позволяет перемещаться между сохранениями.
* ***Git log*** - Выводит список всех коммитов (сохранениий) в хронологическом порядке.
* ***Git diff*** - Показывает разницу между текущей и уже зафиксированной версией файла.
* ***Git add*** - Добавляет версионность файлу в локальном репозитории.
* ***Git commit*** - Фиксирует изменения и сообщает оновых версиях файла.
* ***Git checkout master*** - Возвращает к текущему состоянию работы и позволяет её продолжить.

## Дополнительные команды для работы с ветками
 * ***Git log --graph*** - Позволяет визуализировать поведение веток при вызове комады Get log
 * ***Git Branch*** - Выводит в терминале название всех имеющихся веток и ваше местонахождение среди них.
 * ***Git Branch "Name"*** - Создание новой ветки где "Name" присвоение нового имени.
 * ***Git merge "Name Branch"*** - Команда выполняющая слияние веток, где "Name Branch" имя вливаемой ветки
 * ***Git checkout Branch Name*** - Переийти в указанную ветку
 * ***Git branch -d name branch*** - Удаление ветки

## Порядок действий для настроики работы  с GITHAB
1. _Создаем аккаунт на Github.com_
2. _Создать локальный репозиторий_
3. _"Подружить" локальный и удаленный репозиторий.Github при создании нового репозитория подскажет как это можно сделать. Для этого вам потребуются следущие команды:_
* ***Git remote add origin*** и ссылка с Github на ваш репозиторий - Связывает локальный и удаленный репозитории.
* ***Git branch -M main*** - Команда переименовывает вашу главную ветку которая  будет исползоваться в локальной версии для скачки из удаленного репозитория и загрузки данных с локального репозитория в удаленный в данном случае новое имя (main).
* ***Git push*** - Эта команда позволяет отправить нашу версию репозитория на внешний репозиторий.**ТРЕБУЕТ АВТОРИЗАЦИИ** на вашем репозитории.
4. _Отправить (pull) ваш локальный репозиторий в удаленный (На Github), при этом вам,возможно будет автроризоваться на удаленном репозитории._
* ***Git pull*** - Эта команда позволяет скачать всё из текущего репозитория и автоматически сделать **merge** c нашей версией.
5. _Провести изменения с "другого компьютера"_
6. _Выкачать (pull) актуальное состояние из удаленного репозитория_

## Порядок действий для внесения изменений в удаленный репозиторий
1. _Делаем форк (Fork) интересующего нас репозитория_
* ***Fork*** - Команда полностью копирующая репозитрепозиторий который находится в свободном доступе, но который мы не можем его скачать.
2. _Мы делаем git clone для нашей версии этого репозитория_
* ***Git clone*** - Эта команда позволяет скопировать внешний репозиторий на ваш ПК.
3. _Мы создаем ветку с предлогаемыми изменениями_
4. _Производим все изменения только в этой ветке_
5. _Определяем эти измененияна свой аккаунт (Push)_
6. _В окне на Github появляется возможность отправить (pull request)_
* ***Pull request*** - Загрузить изменные данные в первоисточник.

##  Работа с конфликтами.
При использовагии команды **Git merge** иногда возникают конфликты
![Пример](Конфликт.jpg)
Существует несколько решений сложившейся ситуации:
1. Принять текущие изменения. Это значит оставить все как есть в исходнике.
2. Принять входящие изменения. Приянть изменнения из вливаемой ветки.
3. Принять оба изменения. Значить сохранить текущие отличия в исходнике и прнять входящие одновремено. Можно изменять последовательность. 
4. Сравнить изменения и принять. Тут можно принять оба и дополнить что-то своё, к примеру допечатав собственноручно.  
![Пример](Принятие_решений.jpg)

## Дополнительные команды:
* ***cd*** - Команда которая нужна для определния места корневой  папки котрая будет использоваться нашим репозиторием, после нее пишем имя папки
* ***.Gitignore*** - Файл в который вносятся все элементы которые нужно исключить из списка отслеживания
* ***Clear*** - Команда позволяет отчистить все строки терминала