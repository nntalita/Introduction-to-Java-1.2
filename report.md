# Отчёт о тестировании IntToJava2

## Краткое описание

09.09.2021 - 09.09.2021 было проведено функциональное тестирование  приложения IntToJava2.iml позитивное и негативное.

На тестирование затрачено: 4 часа.

В результате тестирования выявлены следующие дефекты:
* [Result is FAIL при вводе номера карты системы Diners Club - International](https://github.com/nntalita/IntJavaHW2/issues/1#issue-992655790)
* [Result is FAIL при вводе номера карты системы Diners Club - Carte Blanche](https://github.com/nntalita/IntJavaHW2/issues/2#issue-992660981)
* [Result is FAIL при вводе номера карты системы Diners Club - International](https://github.com/nntalita/IntJavaHW2/issues/3#issue-992668641)


## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
* исходники кода;
https://github.com/nntalita/Introduction-to-Java-1.2/blob/16a1aab323e6d2f504c62cdf50cb2a523e2d05c1/src/Main.java


В качестве тестовых данных использовались данные с сайта https://www.freeformatter.com/credit-card-number-generator-validator.html#fakeNumbers:

*Валидные номера карт* - Ожидаемый результат "Result is OK"
* VISA:4716519100150594, 4929376940335288, 4716921646552851902
* MasterCard:5334901834268281, 5536964356130459, 5267074025171572
* American Express (AMEX):378135111350169, 376773444261281,349468128596557
* Discover:6011535927875350, 6011442926043413, 6011176859204662850
* JCB:3528729040827017, 3543264917464604, 3535145857728465148
* Diners Club - Carte Blanche:30316150448268, 30528628083424, 30004173460391
* Diners Club - International:36974760489033, 36370385160218, 36545872674041
* Maestro:6304153938001739, 5018071253693915, 6759031830884313
* Visa Electron:4844544220488000, 4917253291899796, 4844678991350260
* InstaPayment:6379033240745803, 6394284130403737, 6397720790936679

*Невалидные номера карт* -Ожидаемый результат "Result is FAIL"
* +1 к последней цифре валидного номера

Тестирование производилось в следующем окружении:
* Windows 10, версия 20H2 64-разрядная
* JAVA VERSION 11.0.11
