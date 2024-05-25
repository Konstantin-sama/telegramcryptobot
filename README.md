# Telegram bot:
Telegram crypto bot показывает конвертацию валюты в личном чате. База данных - сторонний API.

# Контент: 
'биткоин': 'BTS' 
'эфириум': 'ETH' 
'доллар': 'USD' 

# Описание:
1) При командах /start /help пользователю отправляется краткая информация о том, как пользоваться ботом;
2) При команде /values пользователю отправляется сообщение со списком доступных валют для конвертирования;
3) При вводе текста в формате <имя валюты, цену которой хотим узнать> <имя валюты, в которой надо узнать цену первой валюты> <количество переводимой валюты> пользователю отправляется сообщение с результатом конвертирования заданной волюты.
4) Сообщения об ошибках(например введена неправильная или несуществующая валюта или неправильно введено число) также отправляются пользователю.
5) Парсинг (requests json) для получения курса валют осуществляется через API сайта https://currencylayer.com/documentation. Тариф бесплатный, поэтому кол-во запросов - 1000 в месяц.

# Расположение файлов:
1) Бот и его функции расположены в файле: app.py 
2) Классы и исключения: extensions.py 
3) Токен бота API и переменные с длинным текстом: config.py
