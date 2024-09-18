# Shop

1.Для запуска rabbitmq из контейнера docker ввести команду
    docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.13.7-management
2.Для запуска Celery ввести config(appname)
    celery -A config worker -l info
3. Для запуска Celery c flower ввести команду
    celery -A config flower --basic-auth=login:password
4. test payment Stripe
    successful - 4242 4242 4242 4242 any date future any cvs code
    Failed payment - 4000 0000 0000 0002
    Requires 3D secure authentication 4000 0025 0000 3155