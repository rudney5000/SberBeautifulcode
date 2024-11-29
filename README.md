# DevOps Project: Microservices Deployment and Monitoring

## Описание

Этот проект предназначен для автоматизации развёртывания и мониторинга микросервисной архитектуры. Используются Docker, Kubernetes, Prometheus и Grafana для управления микросервисами и их мониторинга.

## Структура проекта

- **docker-compose.yml** – файл для локального развертывания микросервисов.
- **kubernetes/** – манифесты для развертывания микросервисов в Kubernetes.
- **ci-cd/** – конфигурация CI/CD для автоматизации сборки и развёртывания.
- **monitoring/** – конфигурация для настройки мониторинга с использованием Prometheus и Grafana.

## Установка и запуск

### Локальное развертывание с Docker Compose


Перейдите в директорию проекта:
cd devops-microservices


Запустите Docker Compose:
docker-compose up -d


Откройте браузер и перейдите по следующим адресам:
http://localhost:5001 для доступа к Service A.
http://localhost:5002 для доступа к Service B.
http://localhost:9090 для доступа к Prometheus.
http://localhost:3000 для доступа к Grafana (логин/пароль: admin/admin).
Развертывание в Kubernetes
Настройте доступ к вашему Kubernetes кластеру.
Разверните микросервисы:
kubectl apply -f kubernetes/


Проверьте статусы развёрнутых сервисов:
kubectl get pods
kubectl get services


Настройте доступ к Grafana и Prometheus через NodePort или Ingress.
