# Task_3

### Пишем приложение. Часть 2

1. Новая функция _start_, в которую мы передаем наши переменные _money_, _time_

> function start() {
> <br> &nbsp;&nbsp;&nbsp;&nbsp; money = +prompt('Ваш бюджет на месяц?', '');
> <br> &nbsp;&nbsp;&nbsp;&nbsp; time = prompt('Введите дату в формате YYYY-MM-DD', '2019-06-08');
> <br> }
> <br> start();

2. Делаем проверку для porompt'а _(внутри function start()...)_

> while(isNaN(money) || money == '' || money == null) {
> <br> &nbsp;&nbsp;&nbsp;&nbsp; money = +prompt('Ваш бюджет на месяц?', '');
> <br> }
