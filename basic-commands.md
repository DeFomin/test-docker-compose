# Основные команды для работы с docker compose

Запуск контейнеров ```shell docker-compose up -d ```

Остановка контейнеров ```shell docker-compose up -d ```

Проверка состояния ```shell docker ps -a ```

Очистка сети ```shell docker network prune``` (failed to create network cassandra-cluster_dc1ring: Error response from daemon: Pool overlaps with other one on this address space ) 

Проверка подключения netcat ```shell nc -vz 172.18.0.3 9042 ```

telnet ```shell telnet 172.18.0.3 9042```

Проверка занят ли какой-то определенный порт ```shell sudo lsof -i :9042```

Если требуется удалить все остановленные контейнеры и неиспользуемые образы ```shell docker system prune -a```

Остановить все Docker контейнеры ```shell docker stop $(docker ps -a -q) ``` Опция –q (–quiet) — дает возможно узнавать  идентификаторы самих контейнеров с утилитой ps


Удалить все Docker контейнеры ```shell docker rm $(docker ps -a -q) ```
