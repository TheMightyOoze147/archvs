USAGE:
docker build lab2
docker run -v <path-to-file>:/app/<filename> lab2 /app/main /app/<filename>

Файловая система:
Docker изолирует файловую систему контейнера. Каждый контейнер имеет свою собственную файловую систему, отделенную от хостовой системы.

Процессы:
Каждый контейнер работает в своем собственном пространстве процессов. Это означает, что процессы, запущенные внутри контейнера, изолированы от процессов в других контейнерах и на хостовой системе.

Сеть:
Docker также предоставляет изоляцию сети. Контейнеры имеют свои собственные сетевые пространства, что позволяет изолировать сетевые ресурсы каждого контейнера. Пользователь может определить, какие порты контейнера будут доступны извне.