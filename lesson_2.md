# Домашнее задание к занятию «Базовые объекты K8S»

### Цель задания

В тестовой среде для работы с Kubernetes, установленной в предыдущем ДЗ, необходимо развернуть Pod с приложением и подключиться к нему со своего локального компьютера. 

------

### Чеклист готовности к домашнему заданию

1. Установленное k8s-решение (например, MicroK8S).
2. Установленный локальный kubectl.
3. Редактор YAML-файлов с подключенным Git-репозиторием.

------

### Инструменты и дополнительные материалы, которые пригодятся для выполнения задания

1. Описание [Pod](https://kubernetes.io/docs/concepts/workloads/pods/) и примеры манифестов.
2. Описание [Service](https://kubernetes.io/docs/concepts/services-networking/service/).

------

### Задание 1. Создать Pod с именем hello-world

1. Создать манифест (yaml-конфигурацию) Pod.
2. Использовать image - gcr.io/kubernetes-e2e-test-images/echoserver:2.2.
3. Подключиться локально к Pod с помощью `kubectl port-forward` и вывести значение (curl или в браузере).

------

### Задание 2. Создать Service и подключить его к Pod

1. Создать Pod с именем netology-web.
2. Использовать image — gcr.io/kubernetes-e2e-test-images/echoserver:2.2.
3. Создать Service с именем netology-svc и подключить к netology-web.
4. Подключиться локально к Service с помощью `kubectl port-forward` и вывести значение (curl или в браузере).

------

### Ответ

Выполняла опять на macos и ubuntu:

MacOS:

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240201-tkaa.png)

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240201-tjwt.png)

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240201-tkfq.png)

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240201-tkei.png)

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240202-kpga.png)

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240202-kpas.png)

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240202-kpco.png)

Для curl создала свой сервис и под

Ubuntu:

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240202-kdzk.png)

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240202-kdwg.png)

![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240202-kdxy.png)

Итоговые yml файлы одинаковые, кроме лишнего сервиса под curlpod под макось
[сервисы](https://github.com/Jlljully/k8s/blob/main/files/lesson2/01_service.yaml)  [поды](https://github.com/Jlljully/k8s/blob/main/files/lesson2/01-pod-hello-world.yaml)


+ curl до сервиса

  ![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240202-qncy.png)

  ![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240202-qnbw.png)

  ![Скрин](https://github.com/Jlljully/k8s/blob/main/files/lesson2/SCR-20240202-qmzz.png)
