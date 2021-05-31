# Перечень автоматизированных сценариев


## Позитивные сценарии:

1. Покупка путешествия при помощи дебетовой карты №4444 4444 4444 4441. Кнопка «Купить». Покупка одобрена.
2. Покупка путешествия при помощи дебетовой карты №4444 4444 4444 4441 с опцией «Купить в кредит». Покупка одобрена.
3. Покупка путешествия при помощи дебетовой карты №4444 4444 4444 4442. Кнопка «Купить». Покупка отклонена.
4. Покупка путешествия при помощи дебетовой карты №4444 4444 4444 4442 с опцией «Купить в кредит». Покупка отклонена.

## Негативные сценарии:
1. Покупка путешествия при помощи дебетовой карты №…. отличным от заданных номеров (4444 4444 4444 4441 и 4444 4444 4444 4442). Кнопка «Купить». Покупка отклонена.
2. Покупка путешествия при помощи дебетовой карты №…. отличным от заданных номеров (4444 4444 4444 4441 и 4444 4444 4444 4442). Кнопка «Купить в кредит». Покупка отклонена.
3. Покупка путешествия при помощи дебетовой карты №4444 4444 4444 4441. Ввести некорректные данные в поля: имя и фамилия, срок действия, CVS (при наличии данных полей ввода). Кнопка «Купить». Покупка отклонена.
4. Покупка путешествия при помощи дебетовой карты №4444 4444 4444 4441. Ввести некорректные данные в поля: имя и фамилия, срок действия, CVS (при наличии данных полей ввода). Кнопка «Купить в кредит». Покупка отклонена.
5. Попытка ввода невалидных значений в поля (номер карты, имя и фамилия, срок действия, CVS). Сообщение системы о некорректном виде/формате вводимых данных.
6. Попытка ввода пустых значений в поля (номер карты, имя и фамилия, срок действия, CVS). Сообщение системы о некорректном виде/формате вводимых данных.

## Перечень используемых инструментов с обоснованием выбора
* JetBrains IntelliJ IDEA Ultimate – интегрированная среда разработки программного обеспечения.
* Java, версия 11 – современный язык программирования высокого уровня.
* Gradle — система автоматической сборки, которую используют для упрощения работы с Java.
* JUnit5 –библиотека для модульного тестирования программного обеспечения на Java.
* Selenide – фреймворк для автоматизированного тестирования веб-приложений.
* MySQL – свободная реляционная база данных, обеспечивающаяся поддержкой большого количества типов таблиц.
* PostgreSQL - свободная объективно-реляционная система управления базами данных. 
* Docker – программное обеспечение для автоматизации развёртывания и управления приложениями в средах с поддержкой контейнеризации.
* Allure – фреймворк для создания понятных и простых отчетов автотестов.
* Lombok – библиотека, позволяющая сократить количество написанного кода, улучшая читаемость.

## Перечень и описание возможных рисков при автоматизации
* Проблемы с подключением и настройкой технической части, окружения и СУБД.
* Возможные баги кода.

## Интервальная оценка с учётом рисков (в часах)
* Подготовка и настройка технической части, окружения, СУБД – 15 часов.
* Написание автотестов - 25 часа.
* Выявление и работа с багами, занесение баг-репортов – 8-12 часов.
* Полная отчетность - 14 часов.
* Итоговая оценка - 69 часов.

## План сдачи работ 
* Планирование автоматизации тестирования 08.05.21-11.05.21.
* Подключение и настройка технической части, СУБД, настройка фреймворков 11.05.21-15.05.21.
* Непосредственно сама автоматизация (написание автотестов) 16.05.21-24.05.21.
* Отчеты по итогам автоматизированного тестирования 25.05.21-28.05.21.
* Отчеты по итогам автоматизации 28.05.21-30.05.21.