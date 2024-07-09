# Базовые образы

Различные базовые образы для проектов

## tomcat11manager

Tomcat-11 с менеджером.
Пользователь и пароль tomcat/tomcat.

Сборка образа:
```
docker build -t tomcat11-manager .
```
Пример запуска на порту `8080` на localhost:
```
$ docker run -it -p 8080:8080 --name t11m1 tomcat11-manager
```

