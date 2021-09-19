# Longpoll 3.0.3 beta
## Содержание
1. [Вступление](https://github.com/PAVELNEDELKO1100/phoenix_lp#Вступление)
2. [Установка](https://github.com/PAVELNEDELKO1100/phoenix_lp#Установка)
3. [Команды](https://github.com/PAVELNEDELKO1100/phoenix_lp#Команды)
4. [Архив с лп](https://github.com/PAVELNEDELKO1100/phoenix_lp#Архив)
5. [Запуск](https://github.com/PAVELNEDELKO1100/phoenix_lp#Запуск)
## Вступление

Этот проект был создан в целях популизации использования vk longpoll. Просмотрев данный код, Вы можете взять из него что-то себе,
или взять его как основу для своего проекта. Данный проект требует Python 3.8 и установленные библиотеки vk_api, PyQt5, PySite2. Остальные 
библиотеки уже установленны 

## Установка
Установка не займёт много времени. Достаточно просто установить сами скрипты и установить описанные выше библиотеки.

Для начала запустим консоль и установим все нужные библиотеки:
```bash
pip install -r requirements.txt
```

Всё нужное установлено! Для запуска программы откройте файл start.py.

Токен брать от приложения Kate Mobile - https://vkhost.github.io

## Команды

|Команда|Описание|
|---|---|
|!л пинг / пиу / кинг / п | Показывает задержку скрипта |
|!л инфа | Показывает информацию о дежурном |
|!л -с | Удаляет сообщения дежурного |
|!л -фс / !банхаммер (ссылка, или реплей) | Удаляет сообщения от пользователя (работает только тогда, когда Вы админ в чате |
|!л дд (число) | Скрытно удаляет сообщения (пользователи, которые видят удалённые сообщения, не смогут прочитать ваши удалённые сообщения) |
|!л добавить / вернуть (ссылка) | Добавляет пользователя в беседу |
|!л бан (ссылка, или реплей) | Удаляет сообщения от пользователя и кикает его из беседы |
|!л кто ты (ссылка, или реплей) | Показывает информацию о пользователе |
|!л +др / -др (ссылка, или реплей) | Добавляет, или удаляет из друзей |
|!л +дрв (число) | Добавляет в друзья всю беседу (перед каждым добавлением в друзья будет задержка, которую вы укажите. Желательно ставить задержку в 30 секунд. |
|!л +онлайн / -онлайн | Включает, или выключает вечный онлайн |
|!л +чат / -чат | Добавляет, или убирает в специальные чаты (нужно для авточиталки) |
|!л стч / cпч | Включает, или выключает авточиталку специальных чатов |
|!л +ш / -ш (название (с 1 строки), текст, или фотографии, музыка, документы (со 2 строки) | Добавляет, или убирает шаблоны |
|!л мш | Показывает список ваших шаблонов |
|!л ш | Воспроизводит ваш шаблон |
|!л дшабы | Показывает список всех стандартных дшабов |
|!л (название стандартного дшаба) | Активирует стандартный дшаб |
|!л +дш / -дш | (название (с 1 строки), текст (со 2 строки), при добавлении элемента в дшаб укажите его имя и текст нового элемента) | Добавляет новый дшаб, или добавляет новый элемнт в существующий дшаб, или удаляет дшаб |
|!л мдш | Показывает список ваших дшабов |
|!л эдш (название дшаба) | Показывает элементы дшаба |
|!л рдш (название дшаба, номер элемента (с 1 строки), текст на который нужно изменить элемент (со 2 строки)) | Изменяет текст выбраного элемента |
|!л удш (название дшаба, номер элемента) | Удаляет выбранный элемент |
|!л дш (название дшаба) | Воспроизводит дшаб |
|!л сб (время (если в часах, то !л сб 1 ч, если в минутах, то !л сб 1 м, если в секундах, то !л сб 1) (с 1 строки), текст (со 2 строки)) | Отправляет самоудаляющееся сообщение |
|!л конв (реплей, или текст в самом сообщении) | Переводит сообщение, написанное на английском (пример: Ghbdtn - Привет) |
|!л шрифты | Показывает список доступных шрифтов |
|!л пш (номер шрифта (с 1 строки), текст (только на английском, со 2 строки)) | Изменяет на написанный вами текст с указанным вами шрифтом |
|!л +смс (число (с 1 строки), текст (со 2 строки) | Напишет указанное вами число сообщений с указанным вами текстом |
|!л спам (число (с 1 строки), текст (со 2 строки) | Напишет указанное вами сообщение с указанной вами задержкой (сообщения будут отправляться до капчи) |
|!л ф 1 / ф 2 | Отправит выбранный вами вариант дшаба "ф" |
|!л гб | Отправит дшаб "Го бухать" |
|!л дебаг (реплей) | (нужно для программирования) Покажет список "items" выбранного сообщения |
|!л апи (методы со второй строки, напимер vk.method('messages.send', {'peer_id': peer_id, 'message': "тест", 'random_id': 0, 'disable_mentions': 1,'expire_ttl': 86400}), весь список методов можно посмотреть здесь: https://vk.com/dev/methods | Пригодится для выполнения метода прямо в вк |
|!л дата (дата в формате ДД.ММ.ГГГГ | Изменяет дату регистрации пользователя на ту, что Вы укажите |
|!л +адр (задержка в сек.) / !л -адр | Включает / выключает автоматическую смену даты рождения, если включена - будет менять дату дня раждения на рандомную дату |
|!л статус ((со второй строки) текст, который будет в статусе) | Меняет Ваш статус |
|!л +аст (ваш часовой пояс с разницей по UTC) / !л -аст | Включает / отключает автостату |

Так-же есть скрытые команды, которые смогут найти только те, кто посмотрит сам код.

## Архив
Архив можно скачать тут https://disk.yandex.kz/d/K0telDQ0npB3qw

## Запуск
Запускать командой python3 start.py