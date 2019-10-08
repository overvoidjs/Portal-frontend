# Тестовое задание

## Задание 1

** Backend разработчик реализовал API регистрации со следующими требованиями:**
 

    /catch/catch_registration //Регистрация пользователя

Ожидает получить POST :

    login //str
    password //str
    email //str
    phone //str
    type //если слушатель то '1', если лекционный центр то '2'

---- если type == 1 , так же ожидает получить POST:

    full_name //str format Ф.И.О.
    worker_position //str - Должность
    worker_city //str - город

---- если type == 2 , так же ожидает получить POST:

    full_name //str
    inn //int
    kpp //int
    ogrn //int
    jur_name //str
    jur_address //json str
    fiz_address //json str

**Ваша задача реализовать форму и написать AJAX для передачи данных в API**

----

## Задание 2

У вас есть 5 input полей, необходимо при клике на кнопку **.btn** собрать данные из этих полей и представить их в виде JSON массива.

пример:  
** [ {"id": "1"}, {"id": "2"} , ... ] **

---

## Задание 3

Реализуйте адаптивную верстку данной страницы:

[![Responsive](https://github.com/overvoidjs/Portal-frontend/blob/master/img/Registration/03.jpg "Responsive")](https://github.com/overvoidjs/Portal-frontend/blob/master/img/Registration/03.jpg "Responsive")


