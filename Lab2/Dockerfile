# Используем базовый образ
FROM ubuntu:latest

# Копируем bash-скрипт в контейнер
COPY lb2.sh /usr/src/app/lb2.sh
COPY test.txt /usr/src/app/test.txt

# права на выполнение скрипта
RUN chmod +x /usr/src/app/lb2.sh && apt-get update && apt-get install -y bash net-tools

# Запуск скриптa при старте контейнера
CMD ["/usr/src/app/lb2.sh"]
