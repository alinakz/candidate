Задание к выполнению на должность программиста. (версия 1.0)
=============

* За каждое выполненное требование кандидат получает/не получает баллы соответствующие пункту (указано в скобках);
* Максимальное количество баллов = 100;

## Теория. ##
Кандидат должен отвечать своими словами, иначе баллы не засчитываются:

1. Что такое ООП и для чего оно нужно ? (1б)
2. Что такое наследование, полиморфизм, инкапсуляция ? (1б)
3. Что такое MVC и в чём на Ваш взгляд его основное преимущество ? (1б)
4. Что такое фреймворк ? (1б)
5. Какую реализацию технологии ORM использует фреймворк YII ? (1б)
6. Для чего нужна нормализация баз данных ? (1б)
7. Для чего нужно пространство имен ? (1б)
8. Какие плюсы использования JavaScript в веб-приложении ? (1б)
9. Что такое область видимости переменных ? (1б)
10. Что такое AJAX и в чём на Ваш взгляд его основное преимущество ? (1б)
11. Что такое JSON ? (1б)

## Практика. ##
### Задача №1. ###
#### Описание. ####
* Необходимо написать веб-приложение "Телефонный справочник компании";
* Данные должны храниться в локальной базе данных;
* Неавторизованный пользователь может:
	* видеть интерфейс без расширенных функций;
	* видеть список всех сотрудников в виде таблицы (порядковый номер записи, дата создания записи, ФИО сотрудника, номер телефона, этаж, кабинет);
	* выполнить вход в интерфейс с расширенными функциями через форму авторизации, с введением имя пользователя и пароля;
* Авторизованный пользователь видит интерфейс с расширенными функциями и может:
	* создавать запись (ФИО сотрудника, номер телефона, этаж, кабинет);
	* редактировать запись (ФИО сотрудника, номер телефона, этаж, кабинет);
	* удалять запись;
	* выполнить выход из интерфейса с расширенными функциями;

#### Обязательно к исполнению. ####
* Использовать фреймворк YII (только шаблон "basic") [1]; (1б)
* В качестве базы данных использовать MySQL[1] в кодировке UTF-8; (1б)
* Создание таблиц в базе данных и внесение в них начальных данных должно осуществляться с помощью миграций YII; (2б)
* Файловая структура проекта не должна содержать демонстрационных, тестовых и неиспользуемых директорий и файлов; (3б)
* Фреймворк YII не должен содержать демонстрационных, тестовых и неиспользуемых плагинов и расширений; (2б)
* Девелоперские[2] файлы и классы проекта не должны содержать демонстрационных, тестовых и неиспользуемых переменных, функций и методов; (4б)
* Вывести в заголовок окна браузера дату, когда Вы приступили к выполнению задания, версию задания и версию YII; (1б)
* Исходный код проекта содержит комментарии, разъясняющие назначение основных блоков и строк кода; (5б)
* Интерфейс:
	* должен использоваться широкий подход к построению интерактивных пользовательских интерфейсов с задействованием технологии AJAX; (5б)
	* дизайн должен быть полностью девелоперским, выполненным в одной цветовой схеме, минималистичным; (4б)
	* html-разметка должна соответствовать HTML версии 5; (2б)
	* использовать шрифт Google Roboto; (1б)
	* использовать фреймворк jQuery 2[1]; (2б)
	* все взаимодействия пользователя с интерфейсом осуществляются без перезагрузки страницы, исключение может составить процесс авторизации; (4б)
	* валидация и отправка введенных данных во всех формах осуществляется при помощи JavaScript и AJAX; (4б)
	* форма добавления/редактирования записи в таблицу должна быть выполнена в виде модального окна; (4б)
	* обмен данными с сервером осуществляется в формате JSON; (2б)

#### Рекомендуемое к исполнению. ####
* Функции и методы проекта содержат doc-блоки (PHPDoc, JavaScriptDoc) с наименованием функции/метода, принимаемых переменных, типом возвращаемого значения; (5б)
* Проект должен содержать favicon; (1б)
* Подойти к выполнению задания с энтузиазмом и креативом :) (6б - определяется общим уровнем выполненного задания)
* Девелоперские[2] php код должен быть максимально валидным для версий 5.4+; (2б)
* Девелоперские[2] JavaScript код должен быть максимально валидным для JSLint; (4б)

### Задача №2. ###
#### Описание. ####
* В одном JavaScript-файле необходимо:
	* Написать функцию транслитерации переданной в неё строки; (2б)
	* С использованием прототипов:
		* Расширить базовый объект String методом аналогичным предыдущей функции;  (3б)
		* Написать класс "Автомобиль" со свойствами ("фирма производитель", "модель") и методами ("ехать", "остановиться", "повернуть"); (3б)
		* Написать класс "Легковой" со свойствами ("количество сидячих мест") и методами ("посадить пассажиров", "высадить пассажиров") и унаследоваться от класса "Автомобиль", переопределить наследуемые свойства; (3б)
		* Написать класс "Грузовой" со свойствами ("максимальная грузоподъемность") и методами ("загрузить", "разгрузить") и унаследоваться от класса "Автомобиль", переопределить наследуемые свойства; (3б)
		* Написать класс "Спортивный" со свойствами ("максимальная скорость") и методами ("включить ускорение") и унаследоваться от класса "Легковой", переопределить наследуемые свойства; (3б)
		* Создать экземпляр класса "Грузовой" и вызвать всё доступные ему методы; (2б)
		* Создать экземпляр класса "Спортивный" и вызвать всё доступные ему методы; (2б)

## Общие требования. ##
* Готовый к использованию проект должен быть размещен на хостинге GitHub и доступен для клонирования; (3б)

## Приветствуются навыки и умения. ##
(для подтверждения перечисленных навыков и умений необходимо ответить на приложенные к пунктам вопросы своими словам)
* IDE JetBrains PhpStorm:
	* На какой платформе разработана данная IDE ?
	* Наличие какого ПО необходимо для запуска IDE ?
	* Какова стоимость ключа на 1 год ? [3]
	* Перечислите некоторые возможности IDE;
	* Как называется модальное окно настройки удаленных серверов ?
* ОС семейства Linux:
	* Какие преимущества есть у ОС данного семейства ?
	* Какую графическую оболочку по-умолчанию использует дистрибутив Ubuntu, Debian ?
	* Какой менеджер пакетов они используют? 	
	* Напишите команду поиска файла hosts на локальном компьютере;
	* Напишите команду подключения к удаленному серверу remote.com через порт 2222 под пользователем user1;
	* Напишите команду копирования файла test.php на удаленный сервер remote.com через порт 2222 в директорию /var/www/html по ssh;
* VCS Git:
	* Для чего нужно данное ПО ?
	* Напишите команду клонирования проекта test с удаленного сервера remote.com;
	* Напишите команду создания ветки develop в проекте test и переход в неё;
	* Напишите команду слияние ветки develop в мастер;
* умение работать как в команде так и индивидуально;

[1]: последняя стабильная версия на дату выполнения задания

[2]: созданное разработчиком приложения

[3]: на момент выполнения задания
