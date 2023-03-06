

```terminal
newgrp docker
docker login orgsite:4567
docker run -d -p (свободный порт):5432 --name (имя контейнера) (путь к образу)
```

```terminal
docker container ls - вывести список запущенных контейнеров
docker logs (container_name) - посмотреть логи контейнера

docker system prune --all --force --volumes - удалить все неиспользуемые контейнеры, образы и пр.

docker stop (container_name) - остановить работу конкретного контейнера
docker rm (container_name) - удалить контейнер
```

