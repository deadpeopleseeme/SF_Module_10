Использовал в программе именно decimal формат, т.к. изначально непонятно, какой именно тип числа будет вводить юзер, а decimal даст нам наибольшую точность.

Если всё же нужно использовать обобщенный интерфейс, можно

1) сделать проверку строки от пользователя на содержание "," символа (используем decimal), количество символов (вряд ли мы юзаем short, когда в строке 5 символов) и тд
2) в зависимости от этой проверки передавать в метод, суммирующий 2 числа, число определенного типа, использовать INumber, работающий с любыми числами (https://dev.to/pbouillon/using-inumber-to-generify-math-function-in-net-7-30d3)