# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

28.12.2020 - 28.12.2020 было проведено тестирование установки, функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено 1.5 часа.

В результате тестирования выявлены следующие дефекты:
* [Валидные номера карт длиной меньше или больше 16 символов отмечаются как не валидные при их проверке в приложении Credit Card Number Validator](https://github.com/Cossmoz/Credit-Card-Number-Validator/issues/2)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Руководство по установке IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md)
* Список форматов номеров кредитных карт с сайта https://www.freeformatter.com/credit-card-number-generator-validator.html

В качестве тестовых данных использовались сгенерированные номера карт cо следующих сайтов: [Credit Card Number Generator & Validator](https://www.freeformatter.com/credit-card-number-generator-validator.html), [Dummy Credit Card Generator Cmlabs](https://cmlabs.co/dummy-credit-card-generator/), [Generate for Maestro](https://creditcardgenerator.in/card-generator/maestro). А также данные для негативных тестов.


Номера карт, начинающиеся на 3, длиной 14, 15, 16, 19 символов:
* 30046735238294
* 349335781568506
* 3538841481043281
* 3541321986300924570

Номера карт, начинающиеся на 4, длиной 13, 16, 19 символов:
* 4965023646623
* 4844021811146966
* 4485750109066252073

Номера карт, начинающиеся на 5, длиной 16, 19 символов:
* 5413380484247784
* 5085747645798517099

Номера карт, начинающиеся на 6, длиной 16, 19 символов:
* 6382484667457924
* 6011165888835710559

Данные для негативных тестов:
* 0000000000000000
* 3333333333333333
* пустая строка
* abcdefghijklmnop
* a3c4efgh3jklmnop
* @$%&?"|\()^:;><{


Тестирование производилось в следующем окружении:

* Устройство: Windows 10 Домашняя x64
* Версия java: openjdk 11.0.9.1 2020-11-04