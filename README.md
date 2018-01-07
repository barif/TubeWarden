Инструкция по развертыванию:

* Установить git
* Забрать исходный код:
```
    git clone https://github.com/SHTrassEr/TubeWarden.git
```
* Установить NodeJS 8.9.3+,  MySql
* Создать пустую базу данных в MySql
* Скопировать файл `src/config.example.ts` в `src/config.ts`
* В файле `config.ts` указать параметры подключения к БД, а так же ключ гугла. Инструкция по получению ключа гугла: https://developers.google.com/youtube/v3/getting-started  
* Выполнить команды
```
    sudo npm install -g gulp
    cd TubeWarden/
    npm install
    gulp
    npm start
```
* Для запуска служб сбора статистики нужно выполнить команды:
```
    node bin/script/statisticsGrabberWorker.js
    node bin/script/trendsGrabberWorker.js
```
    
    