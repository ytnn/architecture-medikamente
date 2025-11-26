# Задание 4. Оценка узких мест при миграции

## Диаграмма Исикавы
<img width="2288" height="700" alt="image" src="https://github.com/user-attachments/assets/7d4ce8c1-fa0e-4df5-b908-5ef5f02bb951" />

[Файл xml](https://github.com/ytnn/architecture-medikamente/blob/74c2f55a256ff781318923740e17a068ed8b553c/Task4/Ishikawa.xml)


## Выявленные проблемы и предложенные решения

| Проблема                        | Решение                                          | Приоритет  |
| ------------------------------- | ------------------------------------------------ | ---------- |
| Неправильное разбиение монолита | Выделить bounded contexts                        |  Высокий |
| Отсутствие кеширования          | Внедрить Redis для read-heavy операций           |  Высокий |
| Нет мониторинга                 | Prometheus + Grafana + Jaeger                    |  Высокий |
| Нет CI/CD                       | GitLab CI / GitHub Actions + ArgoCD              |  Высокий |
| Нет нагрузочного тестирования   | Добавить нагрузочные тесты (k6)                  |  Средний |
| Ручные релизы                   | Canary и Blue/Green деплой                       |  Средний |
| Нет знаний у команды            | Обучение DevOps / Обучение разработчиков         |  Средний |
| Нет API Gateway                 | Внедрить Kong / Nginx / Traefik                  |  Средний |



 







