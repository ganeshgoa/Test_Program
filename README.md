# Test_Program
Модули автотестов процедур LTE 
Данная программа автоматически определить успешное завершение процедур:
1) Attach Request / Attach Complete
2) AIR/AIA - обращение к HSS по диаметру
3) Auth Request/Response
4) Security Mode Command / Security Mode Complete
5) Create Session Request / Create Session Response
6) Modify Bearer Request / Modify Bearer Response
7) Release Access Bearer Request / Release Access Bearer Response
8) Delete Bearer Request / Delete Bearer Response

Код находится в файле prod2, трейс в файле s1_gtp2_dia. Оба файла необходимо добавить в одну папку перед запуском. 

Основная суть работы заключается в обращении к содержимому пакетов для извлечения информации об инициации вышеперечисленных процедур, а также об их успешном завершении. 
В некоторых случаях извлечение содержимого пакетов осуществляется с помощью библиотеки pyshark. В других случаях содержимое пакета преобразуется в словарь, затем в список. Затем идёт поэлементное обращение к нужному полю в списке. 
