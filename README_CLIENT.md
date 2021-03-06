 # CLOUD Task Manager 

CLOUD Task Manager - это компактное удобное расширение для Google Chrome, позволяющее работать со списком задач. С ним вы легко сможете осуществить все свои планы и ничего не забыть.  


  - Совершенно бесплатное
  - Личная учетная запись с только ВАШИМИ задачами
  - Синхронизация на других компьютерах, планшетах, ноутбуках
  - Простой, но яркий и удобный интерфейс

# Особенности!

  - Вход под своей учетной записью и регистрация новой
  - Добавление/удаление/редактирование задач
  - Удаление всех выполненных задач за один клик!


### Технические особенности

CLOUD Task Manager использует следующие технологии для корректной работы:

* [JS](js.org) - для взаимодйствия с сервером
* [ASP.net](asp.net) - для создания основы приложения
* [HTML5](http://html5.com/)/[CSS3](css3.com) - для красивого и удобного дизайна
* [jQuery](https://jquery.com)

И, конечно же, CLOUD Task Manager имеет свой [репозиторий](https://github.com/ashette/CLOUD-Task-Manager) на GitHub.  

Некоторые характеристики файлов представлены ниже.


Название файла | Характеристика 
--- | ---
CTMComponent.js  | Компонент, содержащий в себе методы, позволяющие обрабатывать данные для взаимодействия с сервером
login.js| Отвечает за авторизацию пользователя
register.js| Отвечает за регистрацию пользователя
popup.js| Отвечает за основной функционал приложения
cookie.js| Содержит в себе методы для работы с файлами cookie
login.html, register.html,    popup.html | HTML-разметка
style.css,    style_login.css,    style_reqister.css  | Отвечает за стилевые особенности приложения
### CMTComponent.js

Описание методов компонента.

###### Метод регистрации принимает следующие аргументы: 
* email - адрес электронной почты
* password - пароль
* confirmpassword - подтверждение пароля 
* handleSuccess - событие, реагирующие на успешное выполнение функции
* handleFail - событие, реагирующие на неуспешное выполнение функции
``` js
 this.register = function (email, password, confirmpassword, handleSuccess, handleFail){}
```
###### Метод авторизации:  

``` js
 this.login = function (login, password, handleSuccess, handleFail){}
```
###### Метод вывода всех задач пользователя:
* token - содержит в себе токен
``` js
this.getAllTasks = function (token, handleSuccess, handleFail){}
```
###### Метод добавления задачи:
* complete - статус выполнения задачи (true/false). По умолчанию - false
``` js
this.addTask = function (token, complete, text, handleSuccess, handleFail){}
```
###### Метод редактирования задачи: 
``` js
this.editTask = function (token, id, complete, text, handleSuccess, handleFail) {}
```
###### Метод удаления задачи:
``` js
this.deleteTask = function (token, id, handleSuccess, handleFail) {}
```
###### Метод изменения статуса задачи на выполненный:
``` js
this.completeTask = function (token, id, complete, handleSuccess, handleFail) {}
```
###### Метод удаления всех выполненных задач:
``` js
this.deleteCompletedTasks = function (token, handleSuccess, handleFail) {}
```
###### Метод выхода из системы:
``` js 
this.logOut = function (token, handleSuccess, handleFail) {}
```
### Установка
1. Скачайте архив из [репозитория](https://github.com/ashette/CLOUD-Task-Manager)
2. Разархивируйте файл с приложением
2. Откройте браузер Google Chrome
3. Откройте настройку "Управление расширениями"
4. Включите режим разработчика 
5. Нажмите на кнопку "Загрузить распакованное расширение"
6. Выберите папку с приложением и нажмите ОК
7. Готово! Справа на панеле с расширениями появится такой значок:  ![](https://pp.userapi.com/c840439/v840439245/3c0c1/R1cteF5DtX8.jpg)

А так же вы можете скачать данное расширение через [Интернет-магазин Chrome](https://chrome.google.com/webstore/category/extensions?hl=ru).
 
# Разработчики
Студенты УлГТУ, гр. ПиБД-31, г. Ульяновск, 2017 г.


  
