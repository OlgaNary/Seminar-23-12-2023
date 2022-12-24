# Инструкция по работе с Git

## Что такое гит?
***Git*** - самая популярная реализация распределённой системы контроля версий(версионность поддерживается и на сервере, и у каждого клиента). Самой распространнённой реализацией ***Git*** является (GitHub)[https://github.com]

## Подготовка репозитория
Для создания репозитория используется команда *git init*. Для этого необходимо открыть в терминале папку с будущем репозиторием и написать *git init*

## Создание коммитов

### Добавление файлов к коммиту
Для добавления файла к новому коммиту используется команда *git add*. Используется она следующим образом: в терминале с папкой-репозиторием пишем *git add <название файла>*.

### Создание коммита
Для создание новой фиксации(коммита) используется команда *git commit*. Для этого в терминале с папкой-репозиторием пишем *git commit -m "<сообщение к коммиту>*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!!!***

## Журнал изменений
Для просмотра истории изменений используется команда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать *git log*

## Перемещение между коммитами
Для перемещения на другую фиксацию(коммит) используется команда *git checkout*. Для этого необходимо, как показано в прошлом пункте, в журнале изменений найти необходимый коммит и его хеш(номер), после чего в терминале с папкой-репозиторием надо написать *git checkout <хеш коммита>*. После выполнения этой команды мы попадаем в состояние **detached head**, в котором никакие следующие коммиты сохраняться не будут. Для выхода из этого состояния необходимо написать *git checkout master*.

## Ветки в гит
### Создание веток в гит
Для создание новой ветки используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch <название ветки>*.
### Просмотр списка веток
Для просмотра списка веток используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch*. Выделенная зелёным со звёздочкой ветка - это ветка, в данный момент на которой мы находимся.

### Перемещение между ветками
Для перехода на другую ветку используется команда *git checkout*. Для этого в терминале с папкой-репозиторием необходимо написать *git checkout <название ветки>*. Такая ветка должна **существовать**.

## Слияние веток и разрешение конфликтов
Слияние веток происходит следующим образом:
Чтобы слить две ветки используется команда *git merge <имя ветки>*. Для этого нужно, находясь в ветке "чистовика" написать *git merge <имя ветки>*.

При слиянии веток может возникнуть ситуация, когда стратегия Гит не сработает и возникнет конфликт слияния.
Для разрешения конфликта необходимо выбрать один из трех сценариев: *Accept current change / Accept incoming change/ Accept both changes / Compare changes*. Либо внести изменения в тексте вручную.


## Удаление веток
Чтобы удалить ветку используется команда *git branch -d <имя ветки>*. Для этого в терминале с папкой-репозиторием нужно написать: *git branch -d <имя ветки>*.

# Работа с удаленными репозиториями на github

## Скопировать чужой репозиторий в свой аакаунт на github.
Чтобы скопировать чужой репозиторий в свой аакаунт на github, нужно на странице чужого репозитория нажать Fork, и в открывшемся окне надать кнопку Create Fork. После этого копия данного репозитория появится в нашем аккаунте на github.


