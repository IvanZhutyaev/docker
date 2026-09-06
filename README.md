# Docker
<h3>Docker-платформа для разработки доставки и запуска контейнерных приложений</h3>
<b>Docker позволяет создавать контейнеры, автоматизировать их запуск и развертывание, управляет жизненным циклом. Он позволяет запускать множество контейнеров на одной хост-машине</b><br>

## Этапы работы Docker

Docker Engine -> Dockerfile -> Build(Docker Image) -> Run(Docker Container) -> Worked
<br>

    Docker Engine --> Dockerfile;
    Dockerfile --> Build --> Docker Image;
    Docker Image --> Run --> Docker Container;
    Docker Container --> Worked;


**Dockerfile - инструкция для записи образа<br>Docker Image - образ сервиса<br>Docker Container - готовый и развёрнутый контейнер**<br>
<h3>Docker Daemon - это сервер Docker, который ожидает запросов к API Docker. Демон Docker управляет образами, контейнерами, сетями и потоками</h3><br>
<b>Docker Volumes - представляют собой наиболее предпочтительный механизм постоянного хранения данных, потребляемых или производимых приложениями<br>Тома - способ хранения данных<br>Один том может быть примонтирован одновременно в несколько контейнеров. Когда никто не использует том, он не удаляется, а продолжает существовать</b>
<h4>Docker Registry - представляет собой удалённую платформу, используемую для хранения образов Docker</h4>
<h4>Docker Hub - реестр образов Docker</h4>
<h4>Docker Networking - позволяет организовывать связь между контейнерами Docker. Соединённые с помощью сети контейнеры могут выполняться на одном и том же хосте или на разных хостах</h4>

## Команды Docker 
**docker ps(--all/--quiet) - список зап. контейнеров<br>
docker pull - скачать определённый образ или набор образов из Docker Hub<br>
docker build - собирает образ из Dockerfile<br>
docker run - запускает контейнер, на основе указанного образа<br>
docker logs - команда для просмотра логов для указанного контейнера<br>
docker volumes ls - список томов<br>
docker rm - удаляет один и более контейнеров<br>
docker rmi - удаляет один и более образов<br>
docker stop - останавливает один и более контейнеров<br>
docker kill my_container - более грубый способ завершить процесс**

## Docker Compose
<h3>Надстройка над докером, позволяет запускать множество контейнеров и маршрутизировать данные между ними</h3>

### Команды для Docker Compose

**sudo apt install docker-compose - установить docker-compose<br>
docker-compose ps - выводит список контейнеров<br>
docker-compose images - выводит список образов<br>
docker-compose up -d - запустить контейнеры из файла конфигурации<br>
docker-compose -f <docker-compose.yml> up -d - тоже самое, но с указанием файла<br>
docker-compose down - остановить все контейнеры<br>
docker-compose build - только собрать образы, но не запускать контейнеры**