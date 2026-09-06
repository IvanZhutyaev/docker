# Docker
<h3>Docker-платформа для разработки доставки и запуска контейнерных приложений</h3>
<b>Docker позволяет создавать контейнеры, автоматищзировать их запуск и развертывание, управляет жизненным циклом. Он позволяет запускать множество контейнеров на одной хост-машине</b><br>
## Этапы работы Docker
Docker Engine -> Dockerfile -> Build(Docker Image) -> Run(Docker Container) -> Worked
```mermaid
graph TD;
    Docker Engine --> Dockerfile;
    Dockerfile --> Build --> Docker Image;
    Docker Image --> Run --> Docker Container;
    Docker Container --> Worked;
```

**Dockerfile - инструкция для записи образа<br>Docker Image - образ сервиса<br>Docker C
й и развёрнутый контейнер**