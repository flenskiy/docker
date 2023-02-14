# Задание 2

Cборка образа
```
# Команда
sudo docker build -t <image tag> <path to the Dockerfile>

# Пример
sudo docker build -t django_app .
```

Запуск контейнера
```
# Команда
sudo docker run -d -p <port>:<port> --name=<container name> <image tag>

# Пример
sudo docker run -d -p 8000:8000 --name=django-app django_app
```

Логи контейнера
```
# Команда
sudo docker logs  <container name>

# Пример
sudo docker logs django-app
```