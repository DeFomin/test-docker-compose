# Тестовое задание docker compose/cassandra
> Создать Docker Compose скрипт для развертки кластера из трех инстансов cassandra, причем каждый из них должен быть доступен из основной (локальной) сети по отдельному ip адресу.




----------------------------------

Apache Cassandra - это распределенная система управления базами данных (DBMS), относится к классу _NoSQL-систем_ и рассчитанная на 
создание высокомасштабируемых и надёжных хранилищ огромных массивов данных. 

_Обладает гибкой архитектурой_, которая позволяет масштабировать базу данных горизонтально.
То есть добавлять новые узлы в кластер Cassandra для увеличения пропускной способности и хранения больших объемов данных без изменения схемы приложения.

_Обладает высокой доступностью данных_, распределение данных на несколько узлов, обеспечивает автоматическое восстановление данных в случае сбоев. Если один узел становится недоступным, данные все равно остаются доступными через другие реплики
(**репликация данных**).

----------------------------------

Docker Compose - это инструмент для локального развертывания и управления многоконтейнерными приложениями в одном хосте или локальной среде разработки.
В файле конфигурации .yaml/.yml определяются настройки контейнеров, их зависимости и сетевые настройки (_не обеспечивает автоматического балансирования нагрузки и управления масштабированием в крупных распределенных средах._)

**Docker Compose обычно используется для разработки, тестирования и локального развертывания приложений.**
(Kubernetes предоставляет мощные функции управления и оркестрации в распределенных средах. Автоматическое масштабирование, балансировка нагрузки, восстановление после сбоев, управление состоянием приложений)
