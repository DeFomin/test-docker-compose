# Основные команды для работы с docker compose

Запуск контейнеров ```docker-compose up -d ```

Остановка контейнеров ```docker-compose stop ```

Проверка состояния ```docker ps -a ```

Проверка сети ```docker network ls```

Очистка сети ```docker network prune``` (failed to create network cassandra-cluster_dc1ring: Error response from daemon: Pool overlaps with other one on this address space ) 

Проверка подключения netcat ```nc -vz 172.18.0.3 9042 ```

telnet ```telnet 172.18.0.3 9042```

Добавить маршрут ```sudo ip route add <IP-адрес-подсети> via <IP-адрес-машины-А>```

Проверка занят ли какой-то определенный порт ```sudo lsof -i :9042```. Дроп - ```kill {number}```

Если требуется удалить все остановленные контейнеры и неиспользуемые образы ```docker system prune -a```

Остановить все Docker контейнеры ```docker stop $(docker ps -a -q) ``` Опция –q (–quiet) — дает возможно узнавать  идентификаторы самих контейнеров с утилитой ps

Удалить все Docker контейнеры ```docker rm $(docker ps -a -q) ```

Перезапустить систему ```sudo shutdown -r now``` (-r <= restart)
