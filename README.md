1. [План](https://github.com/boog25/Diplom/blob/master/Report/plan.md)
2. [Отчет о тестировании](https://github.com/boog25/Diplom/blob/master/Report/report.md)
3. [Общий отчет](https://github.com/boog25/Diplom/blob/master/Report/SumReport.md)

## Процесс запуска тестов сервиса покупки путешествий для MySql

* Клонирование [репозитория](https://github.com/boog25/Diplom) на компьютер.
* Открыть его с помощью JetBrains IntelliJ IDEA
* Запустить контейнеры MySql и Node c помощью команды docker-compose up -d --force-recreate.
* Проверить запущенные контейнеры командой docker-compose ps.
* Запустить приложение и передать данные для подключения базы MySql командой java -Dspring.datasource.url=jdbc:mysql://localhost:3306/app -Dspring.datasource.username=user -Dspring.datasource.password=pass -Durl="jdbc:mysql://localhost:3306/app" -jar artifacts/aqa-shop.jar
* Запустить тесты командой gradlew clean test -Durl="jdbc:mysql://localhost:3306/app" -Duser="user" -Dpassword="pass" --info
* Сформировать отчет командой gradlew allureServe. 
* Оценить результаты тестирования.

## Процесс запуска тестов сервиса покупки путешествий для PostgreSQL
* Клонирование [репозитория](https://github.com/boog25/Diplom) на компьютер.
* Открыть его с помощью JetBrains IntelliJ IDEA
* Запустить контейнеры PostgreSQL и Node командами docker-compose up -d --force-recreate.
* Проверить запущенные контейнеры командой docker-compose ps.
* Запустить приложение и передать данные для подключения базы PostgreSQL командой java -Dspring.datasource.url=jdbc:postgresql://localhost:5432/appps -Dspring.datasource.username=userps -Dspring.datasource.password=passps -jar artifacts/aqa-shop.jar
* Запустить тесты командой gradlew clean test -Durl="jdbc:postgresql://localhost:5432/appps" -Duser="userps" -Dpassword="passps" --info
* Сформировать отчет командой gradlew allureServe.
* Оцениваем результаты тестирования.
