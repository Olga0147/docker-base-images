# Базовые образы

Различные базовые образы для проектов. 
Аккаунт на Docker Hub : onfocus0147. 

## tomcat11manager

Tomcat-11 с менеджером.
Пользователь и пароль tomcat/tomcat.

Сборка образа:
```
docker build -t tomcat11-manager .
```
Пример запуска на порту `8080` на localhost:
```
docker run -it -p 8080:8080 --name t11m1 tomcat11-manager
```
Пример запуска докер-образа с Docker hub:
```
docker run -it -p 8080:8080 --name t11m1 onfocus0147/tomcat11-manager
```
## tomcat11sample
На образе tomcat11-manager. Содержит в себе sample.war из гайда к tomcat.
Пример запуска докер-образа с Docker hub:
```
docker run -it -p 8080:8080 --name t11m1 onfocus0147/tomcat11-sample
```
