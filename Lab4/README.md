docker-compose up -d
ab -n 10000 -c 10 http://whoami1.docker.localhost/
ab -n 10000 -c 10 http://whoami2.docker.localhost/

curl http://whoami1.docker.localhost/
curl http://whoami2.docker.localhost/
curl http://localhost

localhost в браузере

Traefik:
Traefik - это современный реверс-прокси и балансировщик нагрузки, специально разработанный для работы в контейнерных средах, таких как Docker. Он автоматически обнаруживает новые контейнеры в среде выполнения и настраивает себя соответственно. Traefik поддерживает множество протоколов, включая HTTP, HTTPS, TCP, UDP, и работает с различными системами управления контейнерами.

Whoami:
Whoami - это мини-веб-сервер, который возвращает информацию о себе в ответ на HTTP-запрос. Он часто используется в примерах и тестировании для демонстрации работы реверс-прокси. В данном случае, каждый экземпляр whoami возвращает информацию о себе, например, IP-адрес и данные HTTP-заголовков.

Docker Compose - это инструмент для определения и запуска многоконтейнерных Docker-приложений. Он позволяет определить структуру и параметры всех контейнеров в приложении в файле YAML (docker-compose.yml) и одной командой запустить все контейнеры, настроив их в соответствии с указанными параметрами.