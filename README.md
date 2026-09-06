# Docker
<h3>Docker-платформа для разработки доставки и запуска контейнерных приложений</h3>
<b>Docker позволяет создавать контейнеры, автоматищзировать их запуск и развертывание, управляет жизненным циклом. Он позволяет запускать множество контейнеров на одной хост-машине</b><br>
## Этапы работы Docker
Docker Engine -> Dockerfile -> Build(Docker Image) -> Run(Docker Container) -> Worked
<br>
```mermaid
graph TD;
    Docker Engine --> Dockerfile;
    Dockerfile --> Build --> Docker Image;
    Docker Image --> Run --> Docker Container;
    Docker Container --> Worked;
```

**Dockerfile - инструкция для записи образа<br>Docker Image - образ сервиса<br>Docker Container - готовый и развёрнутый контейнер**<br>
<h3>Docker Daemon - это сервер Docker, который ожидает запросов к API Docker. Демон Docker управляет образами, контейнерами, сетями и потоками</h3>