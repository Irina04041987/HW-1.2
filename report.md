ОТЧЁТ О ТЕСТИРОВАНИИ ПРИЛОЖЕНИЯ CREDIT CARD NUMBER VALIDATOR 
-------------------------------------------------

#### КРАТКОЕ ОПИСАНИЕ ####
 

13.01.2021 было проведено тестирование приемки приложения Credit Card Number Validator для проверки валидации банковской карты. 

**На тестирование затрачено 2 часа**

### В результате тестирования был выявлен баг: 
Некоторые валидные номера карт **платежных систем  "МИР", "Maestro","American Express"**
функционал Credit Card Number Validator отрабатывает неккоректно  и считает их невалидными.

**Баг был заведен в [Issues](https://github.com/Irina04041987/HW-1.2/issues/1).**

#### ОПИСАНИЕ ПРОЦЕССА ТЕСТИРОВАНИЯ ####

В процессе тестирования был проведен запуск кода Credit Card Number Validator в среде INTELLIJ IDEA.

В качестве тестовых данных использовались данные кредитных карт, полученных с сайта :

https://creditcardgenerator.in/:

### Валидные номера карт: ###

**Платежная система МИР**
2204906242619232,
2203887023554872
2203107446868574

**Платежная система American Express**
373134197205624,
370798881826748,
344781317778561

**Платежная система Maestro**
56818642034345132,
503597101304825,
58529822489602

**Ожидаемый результат - результат проверки будет - ОК**

#### ТЕСТИРОВАНИЕ ПРОИЗВОДИЛОСЬ В СЛЕДУЮЩЕМ ОКРУЖЕНИИ: ####

java version "15.0.1"
Windows 7 проф, service pack 1 64 K
INTELLIJ IDEA version 11.0.9
