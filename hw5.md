Создали новый "кластер" main2

![terminal screenshot](screenshot5-1.png)

Создали пользователя для репликации (на скриншоте с ошибкой, но потом она была исправлена). Создали слот. Залили в main дамп базы thai

![terminal screenshot](screenshot5-2.png)
![terminal screenshot](screenshot5-3.png)

Поправили правила доступа к кластеру main

![terminal screenshot](screenshot5-5.jpg)

В остановленном main2 удалили файлы и потом восстановили их из бекапа main и запустили main2

![terminal screenshot](screenshot5-4.png)
![terminal screenshot](screenshot5-6.jpg)

Даем нагрузку на запись, видим 3392tps, смотрим кол-во записей на мастере и реплике - кол-во совпадает

![terminal screenshot](screenshot5-7.png)

Убеждаемся, что не можем делать insert в реплику

![terminal screenshot](screenshot5-8.png)

Был поднят еще один "кластер" main3, в него залит тот же дамп БД thai, и дана такая же нагрузка, как видим 4259tps

![terminal screenshot](screenshot5-9.png)
