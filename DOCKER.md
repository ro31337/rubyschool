Для установки docker системы в linux mint можно использовать скрипт

```
#!/usr/bin/env bash

# https://docs.docker.com/install/linux/docker-ce/ubuntu/
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu xenial stable"
sudo apt-get update
sudo apt-get install docker-ce

# https://docs.docker.com/compose/install/
sudo curl -L https://github.com/docker/compose/releases/download/1.20.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

# https://docs.docker.com/install/linux/linux-postinstall/
sudo groupadd docker
sudo usermod -aG docker $USER
```

Актуальная версия скрипта [тут]:https://gist.github.com/dweldon/39ca0536168a92815a56df44eb55a337

Пример установки docker контейнера с postgres:

1. установка docker контейнера с postgres:
   `docker run --name some-postgres -e POSTGRES_PASSWORD=password -d postgres`

2. Вывести список запущенных контейнеров можно командой:
   `docker ps`
   После выполнения команды в консоли в столбце NAMES отображается имя контейнера "some-postgres"

3. Запуск консоли psql происходит следующей командой
   `docker exec -ti <имя контейнера> psql -U postgres`

После ввода команды появляется приглашение консоли psql
