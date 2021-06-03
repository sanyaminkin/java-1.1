# Отчёт о тестировании валидатора кредитных карт

## Краткое описание

24.05.2021 - 24.05.2021 было проведено функциональное тестирование валидатора кредитных карт.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:
* [Валидатор кредитных карт не принимает некоторые 19-ти значные номера карт Visa, Discover, JCB](https://github.com/sanyaminkin/java-1.1/issues/3)
* [Валидатор кредитных карт не принимает 14-ти значные номера карт Diners Club - Carte Blanche, Diners Club - International](https://github.com/sanyaminkin/java-1.1/issues/2)
* [Валидатор кредитных карт не принимает 15-ти значные номера карт American Express](https://github.com/sanyaminkin/java-1.1/issues/1)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Руководство по установке IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md)






В качестве тестовых данных использовались данные с сайта https://www.freeformatter.com/:
* 16-значные номера карт VISA, Master Card, Discover, JCB, ожидаемый результат - проходят валидацию
* 19-ти значные номер карт Visa, Discover, JCB, ожидаемый результат - проходят валидацию
* 14-ти значные номера карт Diners Club - Carte Blanche, Diners Club - International, ожидаемый результат - проходят валидацию
* 15-ти значные номера карт American Express, ожидаемый результат - проходят валидацию

Тестирование производилось в следующем окружении:
* Windows 7 Ultimate 64-bit
* JDK 11.0.10
* IntelliJ IDEA 2021.1.1
