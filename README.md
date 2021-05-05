# web
```
развертывание веб приложения
Варианты стенда
nginx + php-fpm (laravel/wordpress) + python (flask/django) + js(react/angular)
nginx + java (tomcat/jetty/netty) + go + ruby
можно свои комбинации

Реализации на выбор
- на хостовой системе через конфиги в /etc
- деплой через docker-compose

Для усложнения можно попросить проекты у коллег с курсов по разработке

К сдаче принимается
vagrant стэнд с проброшенными на локалхост портами
каждый порт на свой сайт
через нжинкс
```
В результате проделанных работ было настроено следующее:
- Настроен Vagrant файл и плейбука для ansible которая разоваривает следюущую конфигрурацию:
-  сервис go  висит на localhost:8000 проброшен на nginx 81 порт (https://github.com/mikhail-pavliy/go-http-hello-world)

-  сервис react  висит на localhost:8000 проброшен на nginx 82 порт (https://github.com/mikhail-pavliy/go-http-hello-world)
![image](https://user-images.githubusercontent.com/69155591/117134934-1a39eb80-adc8-11eb-9cf5-80b9118d0794.png)

-  сервис django висит на localhost:8000 проброшен на nginx 83 порт (https://github.com/mikhail-pavliy/django
![image](https://user-images.githubusercontent.com/69155591/117134976-2756da80-adc8-11eb-92dc-3bf3a8f31595.png)
