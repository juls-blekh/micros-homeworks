
# Домашнее задание к занятию «Микросервисы: масштабирование»

Вы работаете в крупной компании, которая строит систему на основе микросервисной архитектуры.
Вам как DevOps-специалисту необходимо выдвинуть предложение по организации инфраструктуры для разработки и эксплуатации.

## Задача 1: Кластеризация

Предложите решение для обеспечения развёртывания, запуска и управления приложениями.
Решение может состоять из одного или нескольких программных продуктов и должно описывать способы и принципы их взаимодействия.

Решение должно соответствовать следующим требованиям:
- поддержка контейнеров;
- обеспечивать обнаружение сервисов и маршрутизацию запросов;
- обеспечивать возможность горизонтального масштабирования;
- обеспечивать возможность автоматического масштабирования;
- обеспечивать явное разделение ресурсов, доступных извне и внутри системы;
- обеспечивать возможность конфигурировать приложения с помощью переменных среды, в том числе с возможностью безопасного хранения чувствительных данных таких как пароли, ключи доступа, ключи шифрования и т. п.

Обоснуйте свой выбор.
### Решение
Есть ряд систем управления кластером, например, Docker Swarm, Apache Mesos, OpenShift и другие, но всё-таки наиболее популярен и пользуется спросом Kubernetes. 
Cоответствие требованиям:
| Параметр\Название | Apache Mesos | OpenShift | Nomand |  Kubernetes|	Docker Swarm|
|---|---|---|---|---|---|
| Поддержка контейнеров | + | + | + | + | + |
| Обнаружение сервисов и маршрутизация запросов | + | + | - | + | + |
| Возможность горизонтального масштабирования | + | + | + | + | + |
| Возможность автоматического масштабирования | + | + | + | + | - |
| Явное разделение ресурсов доступных извне и внутри системы | + | + | + | + | - |
| Возможность конфигурировать приложения с помощью переменных среды | + | + | + | + | + |

Мой выбор в качестве решения для развертывания, запуска и управления приложениями падает на систему оркестрации Kubernetes.

#### Преимущества:

- Самодостаточный инструмент оркестровки, в который встроено множество сервисов. Kubernetes предоставляет все функции, необходимые для запуска приложений на основе контейнеров.
- У Kubernetes самое впечатляющее по числу участников сообщество среди всех оркестраторов, что обеспечивает богатый инструментарий и большое число готовых решений.
- Это бесплатный инструмент с открытым исходным кодом, который работает в любой ОС.


---

### Как оформить ДЗ?

Выполненное домашнее задание пришлите ссылкой на .md-файл в вашем репозитории.

---
