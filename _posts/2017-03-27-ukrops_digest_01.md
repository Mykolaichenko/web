---
layout: post
title:  "UkrOps дайджест #0001"
date:   2017-03-27 20:00:58 +0200
categories: news
---


Новости
-------
[Designing 100G optical connections](https://code.facebook.com/posts/1633153936991442/designing-100g-optical-connections) - Facebook как всегда делают вау-эффект, на этот раз они спроектировали оптику с пропускной способностью в 100 гигабит.  

[Pyston 0.6.1 released, and future plans](https://blog.pyston.org/2017/01/31/pyston-0-6-1-released-and-future-plans/) - Dropbox анонсировал последннюю версию Pyston и больше не будет его девелопить.Они решили вернуться на CPython. Грусть-печаль-тоска.

[Announcing the first SHA1 collision](https://security.googleblog.com/2017/02/announcing-first-sha1-collision.html) - Google доказал несостоятельность криптографического алгоритма SHA1, в общем, выпиливаем.

[Here's how Evernote moved 3 petabytes of data to Google's cloud](http://www.pcworld.com/article/3167594/data-center-cloud/heres-how-evernote-moved-3-petabytes-of-data-to-googles-cloud.html) - Evernote решил отказаться от своих дата-центров, и мувнуться в клауд. Причиной стала незрелая инфраструктура, и несостоявшийся Ops отдел. И вот, через более чем 2 месяца страданий, они это сделали.

[Intent to Deprecate and Remove: Trust in existing Symantec-issued Certificates](https://groups.google.com/a/chromium.org/forum/#!msg/blink-dev/eUAKwjihhBs/rpxMXjZHCQAJ) - Symantec халтурил в проверке личностей/компаний при выдачи EV сертификатов. В Google теперь размышляют, а не перестать ли им доверять после этого.


Процессы
--------
[The Biggest and Weirdest Commits in Linux Kernel Git History](https://www.destroyallsoftware.com/blog/2017/the-biggest-and-weirdest-commits-in-linux-kernel-git-history) - Вся боль использования SVC в больших опен-сорс проектах. Лучше это не читать, ужас, ужас! Пример на базе Linux kernel, кстати.

[DevOps and Continuous Integration challenges in C/C++ projects](http://blog.conan.io/2017/03/14/Devops-and-Continouous-Integration-Challenges-in-C-C++-Projects.html) - Суровый гайд для настоящих профессионалов по настройке процессов CI/CD в среде с C++.


Мнения
------
[Вброс о эволюции](https://ukrops.slack.com/archives/dev_random/p1489648547087416) - Очень качественный вброс от @astlock.

[Ship Small Diffs](https://blog.skyliner.io/ship-small-diffs-741308bec0d1) - И правда, давайте деплоить почаще, маленькими итерациями? 

[Queues Don't Fix Overload](http://ferd.ca/queues-don-t-fix-overload.html) - Старая, но концептуальная и актуальная статья о том, почему менеджеры очередей не решают проблему с чрезмерной нагрузкой на работающую систему.


Туториалы
---------
[The million dollar engineering problem](https://segment.com/blog/the-million-dollar-eng-problem/) - Пост описывает оптимизации использования AWS ресурсов и как компания уменьшила косты для сервисов. В осном речь идет о DynamoDB, Autoscalling, ELB, ECS

[Microservices Workshop All Topics Deck](https://www.slideshare.net/adriancockcroft/microservices-workshop-all-topics-deck-2016) - Концептуальные слайды о микросервисах, архитектуре, проблемах, решениях.

[Auto-Scaling Jenkins with Kubernetes](http://www.monkeylittle.com/blog/2017/02/09/autoscaling-jenkins-with-kubernetes.html) - Как говориться, Jenkins и Kuber - one love. Автор показывает как сетапить ферму из Jenkins в контейнерах.

[Here’s How You Start Using Docker/](http://djangostars.com/blog/heres-how-you-start-using-docker/) - Getting started in Docker. Статья описывает как и что делать, увидев докер первый раз. 


Тулзы
-----
[Top-like interface for container metrics](https://github.com/bcicen/ctop) - Ещё один *top, но теперь специально для контейнеров.

[Synchronize your DNS to multiple providers](https://github.com/StackExchange/dnscontrol) - Новая тула для управления DNS у нескольких провайдеров. Правда непонятно, чем она лучше терраформа.


Linux
-----
[Two frequently used system calls are ~77% slower on AWS EC2](https://blog.packagecloud.io/eng/2017/03/08/system-calls-are-much-slower-on-ec2/) - Интересное исследование на тему того почему некоторые сисколы в AWS медленные. Хороший пример методики исследования.

[Efficient File Copying On Linux](https://eklitzke.org/efficient-file-copying-on-linux) - Cказ о том, почему GNU `cp` копирует блоками по 128 KB и это хорошо

[How to stop Ubuntu Xenial from randomly killing your big processes](https://blog.meteor.com/how-to-stop-ubuntu-xenial-from-randomly-killing-your-big-processes-4a3e2d09323f) - Ubuntu, перестань убивать процессы! Глубокий мануал в Linux internals как контролировать это поведение.


Падения
-------
[A collection of postmortems](https://github.com/danluu/post-mortems) - Великолепная колекция разборов полетов от ведущих компаний (и их вещущих падений).

[Summary of the Amazon S3 Service Disruption](https://aws.amazon.com/ru/message/41926/) - Официальная сводка информации по поводу падения Amazon S3, который заафектил все, что только можно было заафектить.
