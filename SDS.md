# Software Design Specification

### Содержание
1. [Введение](#1)<br>
1.1 [Цель](#1.1)<br>
1.2 [Объем](#1.2)<br>
1.3 [Определения, акронимы и сокращения](#1.3)<br>
2. [Системный обзор](#2)<br>
3. [Соображение по дизайну](#3)<br>
3.1 [Общие ограничения](#3.1)<br>
3.2 [Цели и рекомендации](#3.2)<br>
3.3 [Методология разработки](#3.3)<br>
4. [Архитектурная стратегия](#4)<br>
5. [Дизайн высокого уровня](#5)<br>
6. [Диаграмма классов](#6)<br>
7. [Use cases](#7)<br>




## 1. Введение <a name="1"></a>

### 1.1 Цель <a name="1.1"></a>
Целю данного документа является представить подробное описание медиплеера. Здесь будут описаны программные средства и решения для реализации проекта.

### 1.2 Объем <a name="1.2"></a>
Документ по дизайну программного обеспечения продемонстрирует, как дизайн будет выполнять функциональные и нефункциональные требования, зафиксированные в спецификации требований к программному обеспечению (SRS). Документ предоставит платформу программистам посредством описания компонентов высокого уровня и архитектуры, подсистемы, интерфейса, дизайн базы данных и дизайн алгоритма. Это достигается за счет использования архитектурных паттернов, паттернов проектирования, диаграмм базы данных, диаграмм классов, реляционных модели и пользовательские интерфейсы.

### 1.3 Определения <a name="1.3"></a>
* Пользователь - человек, использующий систему
* Архитектурный дизайн - установление общей структуры программного комплекса

## 2. Системный обзор <a name="2"></a>
Данное приложение представляет собой медиаплеер с понятным интерфейсом. Данное приложение позволяет просматривать медиафайлы. Кроме того, приложение позволяет изменять цвет изображения дя удобства пользователя.

## 3. Соображения по дизайну <a name="3"></a>
Для работы приложения у пользователя должен быть компьютер с установленной операционной системой Windows.

### 3.1 Общие ограничения <a name="3.1"></a>
* Приложение полностью реализовано с использованием фреймворка QT.

### 3.2 Цели и рекомендации <a name="3.2"></a>
* Система должна быть полностью функциональна в запланированные сроки
* Интерфейс должен был интуитивно понятным для базового пользователя

### 3.3 Методология разработки <a name="3.3"></a>
Этот проект осуществляется с использованием модифицированной парадигмы водопада. 
Процесс разработки выглядит как поток, последовательно происходящей фазы анализа требований, проектирования, реализации, тестирования, интеграции и поддержки. 
Так же возможен возврат при разработке на предыдущий этап и рассмотрение модификации решения.

## 4. Архитектурная стратегия <a name="4"></a>
На архитектуру и дизайн повлияли следующие дизайнерские решения и стратегии:
* В дизайне используются объектно-ориентированные принципы (ООП). Компромисс увеличения накладных расходов на код и объектная передача сообщений считается оправданной за счет модульности функциональности, данных инкапсуляция, связь через интерфейсы и повторное использование через полиморфизм
* Для пользователя интерфейс будет представлен в качестве дилогового окна.
* Используемые паттерны: Builder, MVC, Singleton, Abstract Factory, Command, Proxy, Filter Chain, Object pool.

## 5 Дизайн высокого уровня <a name="5"></a>
* [Главное окно](https://github.com/Stasko-Sergey-850504/MePlayer/blob/master/Mockups/main_window.jpg)
* [Дилоговое окно открытия файлов](https://github.com/Stasko-Sergey-850504/MePlayer/blob/master/Mockups/open_window.png)
* [Управление цветом картинки и видео](https://github.com/Stasko-Sergey-850504/MePlayer/blob/master/Mockups/colour_opts.jpg)

## 6 Диаграмма классов <a name="6"></a>
![Диаграмма классов](https://github.com/Stasko-Sergey-850504/MePlayer/blob/master/Diagrams/Class_diagram/class_diagram.md)

## 7 Use cases <a name="7"></a>
![use case](https://github.com/Stasko-Sergey-850504/MePlayer/blob/master/Diagrams/Use_case/Use_case.md)