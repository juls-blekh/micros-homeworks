# Домашнее задание к занятию «Введение в микросервисы»

## Задача 1: Интернет Магазин

Руководство крупного интернет-магазина, у которого постоянно растёт пользовательская база и количество заказов, рассматривает возможность переделки своей внутренней   ИТ-системы на основе микросервисов. 

Вас пригласили в качестве консультанта для оценки целесообразности перехода на микросервисную архитектуру. 

Опишите, какие выгоды может получить компания от перехода на микросервисную архитектуру и какие проблемы нужно решить в первую очередь.

---

### Как оформить ДЗ?

Выполненное домашнее задание пришлите ссылкой на .md-файл в вашем репозитории.

---
### Выгоды от перехода на микросервисную архитектуру  
- Распределение разных бизнес-функций на разные независимые сервисы   
- Использование разных технологий для разных сервисов   
- Масштабируемость системы в соответствии с потребностями
- Более легкое и быстрое внедрение изменений за счет того, что можно делать доработки, исправления, выкладки обновлений для каждого сервиса отдельно
- При развитии просто добавить новый фунционал добавлением нового микросервиса

### Проблемы, которые необходимо решить в первую очередь
- Система усложнится, поэтому возможно увеличение штата, повышение квалификационных требований к сотрудникам.
- Потребуется проработка системы разработки, внедрения, поддержки и сопровождения (версионирование, артефакты, составление документации, автоматизация сборки и тестирования, совместимость сервисов) 
- Проблемы эксплуатации (сбор логов, метрик, их анализ; управление инфраструктурой)  
- Разделение на сервисы таким образом, чтобы она не была наносервисной
- Определение правил межсервисного взаимодействия
