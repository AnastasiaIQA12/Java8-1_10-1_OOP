# Домашнее задание к занятию «Объектно-ориентированное программирование и проектирование»
## Задача №1 - "Радиоман"

### Легенда
В рамках проекта по созданию "Умного дома" у нас появился очень важный клиент, которых хочет кастомную доработку: он очень любит радио, поэтому нам нужно научиться управлять радио.

Что нужно: создать класс `Radio`, в котором хранятся следующие поля (т.е. данные, которые будут помнить о себе объекты радио):
1. Номер текущей (прослушиваемой) радиостанции
1. Громкость звука

Требования к работе с радиостанциями:
1. Номер текущей радиостанции изменяется в пределах от 0 до 9
1. Если текущая радиостанция - 9 и клиент нажал на кнопку `next` (следующая) на пульте, то текущей должна стать 0-ая; в остальных случаях радио переключается просто на следующую станцию. (создайте отдельный метод для этой операции)
1. Если текущая радиостанция - 0 и клиент нажал на кнопку `prev` (предыдущая) на пульте, то текущей должна стать 9-ая; в остальных случаях радиоипереключается просто на предыдущую станцию/ (создайте отдельный метод для этой операции)
1. Клиент должен иметь возможность выставлять номер радиостанции через прямое указание её номера (сделайте сеттер с проверкой на допустимость номера станции)

Требования к работе с уровнем громкости звука:
1. Клиент должен иметь возможность увеличивать и уменьшать уровень громкости звука (в пределах от 0 до 10)
1. Если уровень громкости звука достиг максимального значения, то дальнейшее нажатие на `+` не должно ни к чему приводить (создайте отдельный метод для этой операции)
1. Если уровень громкости звука достиг минимального значения, то дальнейшее нажатие на `-` не должно ни к чему приводить (создайте отдельный метод для этой операции)

**Важно**: один вызов метода должен приводить к переключению на одну радиостанцию!

Создайте на базе проекта с лекции собственный проект, в котором:
1. Подключите плагин Surefire так, чтобы сборка падала в случае отсутсвия тестов
1. Подключите плагин JaCoCo в режиме генерации отчётов (обрушать сборку по покрытию не нужно)
1. Реализуйте нужные классы и методы
1. Напишите автотесты на методы, содержащие логику, добившись 100% покрытия по branch'ам
1. Подключите CI на базе Github Actions и выложите всё на Github

**Итого**: должен быть репозиторий на GitHub, в котором расположен ваш Java-код.

