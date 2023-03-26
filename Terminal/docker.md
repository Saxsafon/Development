### Запуск контейнеров
```terminal
newgrp docker
docker login orgsite:4567

docker run -d -p (свободный порт):5432 --name <имя_контейнера> <путь к образу>
docker-compose up -d --build - построить контейнер/контейнеры через файл docker-compose
```

### Обзор контейнеров
```terminal
docker container ls - вывести список запущенных контейнеров
docker logs <имя_контейнера> - посмотреть логи контейнера
docker logs --follow <имя_контейнера> - посмотреть логи контейнера с обновлением
```

### Подключение к контейнерам
```terminal
docker exec -t -i <имя_контейнера> /bin/bash - подключиться к файловой системе контейнера
docker exec -it <имя_контейнера> psql -U <имя_пользователя> -d <имя_базы_данных> - подключиться к базе данных в контейнере
```

### Остановка и удаление контейнеров
```terminal
docker stop (container_name) - остановить работу конкретного контейнера
docker rm (container_name) - удалить контейнер

docker system prune --all --force --volumes - удалить все неиспользуемые контейнеры, образы и пр.
```


