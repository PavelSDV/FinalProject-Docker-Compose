# FinalProject
Ссылка Django образа: 
https://hub.docker.com/layers/pavelsdv/testrep/projectcompose_web/images/sha256-dd74af69cd7eab088d0354883b1bc66ec3b0bf214e2c8d7a8a0f355ae74b94c7?context=repo

Ссылка Nginx образа: 
https://hub.docker.com/layers/pavelsdv/testrep/projectcompose_nginx/images/sha256-0d048d68a9124ec24ac1365799ee5ba76f9469d7e0846183efd24601eeb03c17?context=repo

Команда для запуска проекта: sudo docker-compose -f docker-compose.yml up -d --build

Админ-панель по адресу: http://127.0.0.1:1337/admin/

Для входа в админ-панель создать суперпользователя: sudo docker-compose run web python3 manage.py createsuperuser

-------------------
Задание.

Задача
Как системному администратору данной организации вам поставлена задача собрать на докер образ Django (Linux, nginx, Django, Postgres, Gunicorn) сервера, который можно было бы выложить в публичный доступ на Docker Hub, предоставляя кандидату только ссылку на образ и команду для установки. Все нужные сервисы должны быть проброшены на хост по стандартным портам, реализация HTTPS не требуется, версии Django, nginx и Postgres не имеют значения, как и версия ядра Linux. В проекте просто должна работать админка с заранее прописанным логином и паролем.

Советы
Образ должен быть загружен как публичный, заведите вторую учётку на Docker Hub (или попросите коллегу проверить доступность).
Не следует использовать для решения Compose, работайте с чистым Docker, у решения задачи Compose много неприятных нюансов.
Есть специальные образы с Python, Django и Gunicorn.
Очень рекомендуем, когда закончите работу над образом и будете готовы его отправить, скачать и развернуть на чистой машине. Кэши иногда работают крайне неприятно, может оказаться, что выгруженная сборка работает не так, как текущая.

-----------------
Итоговая оценка.

Вы уверенно справились с заданием и получаете максимальный балл.

Плюсы:
- Вы грамотно применили полученные знания.
- Вы хорошо освоили основные аспекты применения технологии контейнеризации.
- Команда для разворачивания образа отрабатывает корректно.
- Служба django запущена в контейнере.
- Приложение использует СУБД PostgreSQL.
- Админка отображается и доступна.

Ошибки:
- Не обнаружены.

Поздравляю с успешным завершением курса! Удачи!

Проверку выполнила ментор Миллер Алиса. По возникшим вопросам обращайтесь в каналы блока
"Devops".
