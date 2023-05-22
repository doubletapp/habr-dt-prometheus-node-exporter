# Doubletapp Node Exporter

Docker-compose с единственным сервисом `prometheus/node-exporter`

## Запуск

1. Создать файл .env
    ```
    $ make env
    ```

    `HOST_MACHINE_PORT` - порт экспортера на хосте
2. Запустить приложение
    ```
    $ make
    ```

```
    $ curl 0.0.0.0:${HOST_MACHINE_PORT}/metrics
    # HELP go_gc_duration_seconds A summary of the pause duration of garbage collection cycles.
    . . .
```
