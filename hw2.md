1-8) 
![terminal screenshot](hw2_0.png)

9) Вторая транзакция не видит изменений сделанных первой, потому что они не закомичены

10-11)
 ![terminal screenshot](hw2_1.png)

12) Теперь изменения закомичены и видны второй транзакции

13-12)
 ![terminal screenshot](hw2_2.png)

17) Новую запись не видим. Repeatable read более высокий уровень изоляции чем read committed, следовательно проблема чтения не закомиченых данных на нём тоже не возникает

18-19)
 ![terminal screenshot](hw2_3.png)

20) Запись не видим, потому что при уровне изоляции repeatable read в транзакции будут видны данные закомиченные до начала этой транзакции