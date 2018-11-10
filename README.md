# Veter9_microservices
Veter9 microservices repository

## Выполнение ДЗ 12, Docker-1

- установил докер stable версию
- запустил пару контейнеров
- поигрался с командами
- сделал вывод docker images в лог файл


## Выполнение ДЗ 13, Docker-2
- создал новый проект docker-211709
- подключил gcloud к новому проекту
- создаю хост докер демона на гугле
- пришлось установить докер-машин пакет
- переключаю докер на работу с демоном на гугле
- добавил 4 новых файла в папку docker-monolith
- заполнил их дефолтным конфигом из gist
- приступил к работе над докерфайлом
- сделал первый билд
- первый коммит
- запустил свой контейнер
- добавил новое правило файрвола, но ничего не заработало
- промучался с файрволом
- не разобрался, порт 9292 закрыт. продолжил дальше
- зашел на докерхаб
- включил аутентификацию на докерхабе
- повесил таг и сделал пуш на докерхаб

- проверил на другой машине

## Выполнение ДЗ 14, docker-3
- скачал архив, разместил его в корне репозитория и переименовал
- создал новый бранч и сделал чекаут
- добавил все файлы в гит(git add )
- добавил интеграцию с трависом-
- добавил три докерфайла
- скачал последний образ монги и собрал образы
- создал сеть для приложения (бридж, как я понимаю)
- запустил 3 конетйнера
- ничего не работает. разбираюсь
- сделал коммит, пока всё не поломал (слайд 15)
- а потом заработало

## забыл добавить описание трех ДЗ, вспоминать уже не буду...

## выполнение ДЗ 20, monitoring-2
- выполнил всё, ак по слайдам.
- добавил три правила файрвола
gcloud compute firewall-rules create cadvisor-default --allow tcp:8080
gcloud compute firewall-rules create grafana-default --allow tcp:3000 
gcloud compute firewall-rules create alertmanager-default --allow tcp:9093 
- ссылки на докерхаб
https://hub.docker.com/r/veter9/ui/
https://hub.docker.com/r/veter9/comment/
https://hub.docker.com/r/veter9/post/
https://hub.docker.com/r/veter9/prometheus/
https://hub.docker.com/r/veter9/alertmanager/

# Выполнение ДЗ 21, logging
- выполнил дз по слайдам
- добавил правила файрвола
gcloud compute firewall-rules create elasticsearchudp-default --allow udp:9200
gcloud compute firewall-rules create f luentdtcp-default --allow tcp:24224
gcloud compute firewall-rules create fluentdup-default --allow udp:24224
gcloud compute firewall-rules create kibana-default --allow tcp:5601
gcloud compute firewall-rules create kibanaudp-default --allow udp:5601
- добавил строчку RUN apk update && apk add gcc && apk add musl-dev в докерфайл POST-PY 
- пришлось везде ставиь теги на имаджи эластиксёрч и прочее. Имадж latest он не понимает :)
- 

# выполнение дз 22, kubernetes-1
- поднял кубер через хардвей)
- по ходу задания поменял регион гугл на asia-east2 (иначе не работало)
- так же пришлось сделать apt-get update на нодах для установки nginx(этого в мануале не было)



