# 使用 RabbitMQ 官方镜像
FROM rabbitmq:3.8-management

# 更新软件包并安装 curl
RUN apt-get update && apt-get install -y curl

# 下载并安装 rabbitmq_delayed_message_exchange 插件
RUN curl -L -o /plugins/rabbitmq_delayed_message_exchange.ez \
    https://github.com/rabbitmq/rabbitmq-delayed-message-exchange/releases/download/v3.8.0/rabbitmq_delayed_message_exchange-3.8.0.ez

RUN rabbitmq-plugins enable rabbitmq_delayed_message_exchange
