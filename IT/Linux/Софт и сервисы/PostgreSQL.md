*Все команды выполняются в bash! не в shell СУБД*
Узнать версию СУБД
```
sudo -u postgres psql -tAc "SHOW server_version;"
```
*Более подробный вывод*
```
sudo -u postgres psql -tAc "SELECT version();"
```

Посмотреть запущенные кластеры
```
pg_lsclusters
```
Все процессы `postgres`
```
pgrep -a postgres
```

## TimescaleDB Расширение
Узнать версию установленного расширения
```
psql -U postgres -d postgres -c "SELECT default_version, installed_version
 FROM pg_available_extensions
 WHERE name = 'timescaledb';"
```



## Создание \ Удаление БД

## Создание \ Удаление БД

## Создание \ Удаление БД

## Создание \ Удаление БД
