# Система учета для медицинской организации.

Начало
Эти инструкции позволят вам запустить копию проекта на вашем локальном компьютере. 


## Для начало утановки, Вам будет необходимо:

>Установить Python3: https://pythonworld.ru/osnovy/skachat-python.html
   
## Установка
Пошаговая серия примеров, которые расскажут, как запустить среду разработки.

Создание виртуального окружения

venv Устанавливать venv не нужно, т.к. он входит в стандартную библиотеку Python. Т.е. если вы установили себе Python, то venv у вас уже есть. Помните, что venv работает только в Python3! Для создания виртуального окружения с именем PRG2 с помощью venv в директории проекта выполните следующую команду:

```sh
$ python -m venv PRG2
```
Активация виртуального окружения в директории проекта на Linux выполняется командой:

```sh
$ source PRG2/bin/activate
```

на Windows

>PRG2\Scripts\activate.bat
Установка зависимостей из requirements.txt:

```sh
$ pip3 install -r requirements.txt
$ pip3 install whitenoise
```


## Выполните миграции


>Для Linuxa

```sh
$ python3 manage.py makemigrations
$ python3 manage.py migrate
```
>Для Windowsa

```sh
$ python manage.py makemigrations
$ python manage.py migrate
```

python3 manage.py createsuperuser

## для востановление пароля пользователя, укажите почту отправления в settings.py:
```sh
$ EMAIL_HOST_USER = 'xxxx@gmail.com'
$ EMAIL_HOST_PASSWORD = 'xxxx'
```
