Project Maven Setup

Описание проекта

Этот репозиторий создан для практики написания и настройки файла pom.xml для проекта на Maven. Основной задачей было подключение зависимостей, конфигурирование плагинов для компиляции и сборки, а также настройка запуска JavaFX приложения.

Структура pom.xml

Основные разделы pom.xml:

	•	Зависимости:
	•	Apache Commons Lang: библиотека commons-lang3 для работы с утилитами и вспомогательными классами Java.
	•	JavaFX Controls: библиотека javafx-controls для работы с JavaFX графическим интерфейсом.
	•	JUnit: библиотека junit-jupiter-api для модульного тестирования (в scope test).
	•	Desktop Game Engine: пример игровой библиотеки desktop-game-engine-id.
	•	Плагины:
	•	Maven Compiler Plugin: компиляция кода с использованием версии Java 18.
	•	JavaFX Maven Plugin: для запуска JavaFX-приложения из Maven (указан путь к классу RacerGame).
	•	Maven Jar Plugin: сборка проекта в JAR-файл, добавление зависимостей в сборку и конфигурация класса JarRsrcLoader для запуска.
	•	Maven Dependency Plugin: копирование зависимостей в директорию lib/.
	•	Maven Install Plugin: для распаковки JAR-файлов в зависимости проекта.
	•	Maven Surefire Plugin: запуск тестов и исключение тестов, указанных в списке исключений (например, StrangeTest).
