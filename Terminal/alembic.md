```terminal
Запускается из файла src

alembic revision -m "revision_name"
alembic upgrade head - обновление базы до следующей версии # (вместо head можно указывать номер ревизии)
alembic downgrade head - откат базы до предыдущей версии # (вместо head можно указывать номер)

down_revision - полезно когда нужно откатиться на несколько ревизий)
alembic history - история обновлений базы
alembic current - текущая версия базы
```