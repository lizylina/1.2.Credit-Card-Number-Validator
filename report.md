# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

14.06.2020 г. было проведено позитивное и негативное функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 1 час.

В результате тестирования выявлены следующие дефекты:
* https://github.com/lizylina/1.2.Credit-Card-Number-Validator/issues/1

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* баг-репорты;
* данный отчет о тестировании.

В качестве тестовых данных использовались номера карт различных платежных систем, сгенерированные на сайте [freeformatter.com](https://www.freeformatter.com/credit-card-number-generator-validator.html):
* VISA: 4485375006305806104, ожидаемый результат - "Result is OK"
* MasterCard: 5150909628607904, ожидаемый результат - "Result is OK"
* American Express (AMEX): 347164171336478, ожидаемый результат - "Result is OK"
* Discover: 6011445215320715, ожидаемый результат - "Result is OK"
* JCB: 3535726776845206, ожидаемый результат - "Result is OK"
* Diners Club - North America: 5599003495983272, ожидаемый результат - "Result is OK"
* Diners Club - Carte Blanche: 30526185405600, ожидаемый результат - "Result is OK"   
* Maestro: 586824160825533338, ожидаемый результат - "Result is OK"
* Visa Electron: 4917863804009582, ожидаемый результат - "Result is OK"
* InstaPayment: 6392994304459867, ожидаемый результат - "Result is OK"
* 491786380400958a, ожидаемый результат - "Result is FAIL"
* 515090962*607904, ожидаемый результат - "Result is FAIL"

Тестирование производилось в следующем окружении:
* Версия и разрядность ОС: Windows10 x64
* Версия Java: openjdk version 11.0.7
