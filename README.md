# Генератор коротких ссылок
Скрипт для генериации коротких ссылок с сервиса [bitly.com](https://bitly.com), а также проверки их на переходы.  
Python3 должен быть уже установлен. Затем используйте pip (или pip3, есть конфликт с Python2)
## Установка
```commandline
git clone https://github.com/Weffy61/get_short_link_with_args
```
## Установка зависимостей
Переход в директорию с исполняемым файлом и установка
```commandline
cd get_short_link_with_args
```
```commandline
pip install -r requirements.txt
```
## Получение токена
Зарегистрируйтесь на [bitly.com](https://bitly.com)  
Перейдите по [ссылке](https://app.bitly.com/settings/api/) или вручную `Settings > API`  
Нажмите на кнопку `Generate token` и скопируйте полученный токен
## Настройка
Создайте в корне папки `get_short_link_with_args` файл `.env`. Откройте его для редактирования любым текстовым 
редактором.  
`BITLY_TOKEN='вставить скопированный токен'`
## Запуск
```commandline
python main.py YOUR_URL
```
Замените `YOUR_URL` на ссылку для получение bitly ссылки.  
Замените `YOUR_URL` на bitly ссылку, без указания протокола(HTTP, HTTPS), для получения колличества переходов по ней.
## Помощь
```commandline
 python main.py --help
```
## Цель проекта
Код написан в образовательных целях на онлайн-курсе для веб-разработчиков dvmn.org.