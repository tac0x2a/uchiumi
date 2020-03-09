# Biwako

[![Biwako](./doc/img/biwako.svg)](https://github.com/tac0x2a/biwako)

Biwako is an all in one micro Data Lake for IoT data.


# Services

## [RabbitMQ](https://www.rabbitmq.com/)
Message broker service. The MQTT port listen json format messages. Its general entry point of data stream to Biwako.
+ 15672: Web management console. Default account is `guest`:`guest`.
+ 1883: MQTT port.

## [Grebe](https://github.com/tac0x2a/grebe)
Grebe is forwarder JSON message from RabbitMQ to Clickhouse.

## [ClickHouse](https://clickhouse.tech/)
ClickHouse is a free analytics DBMS for big data. Central data storage of Biwako.
Default database is `default`, and user name and password is `default`.
+ 8123: HTTP client port.

## [Portainer](https://www.portainer.io/)
Portainer is a lightweight management UI. After login, please select `Local` and press `Connect` button.
+ 9000: Web interface.