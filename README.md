# Task_3

### Пишем приложение. Часть 2

1. Новая функция **start**, в которую мы передаем наши переменные _money_, _time_

> function start() {
> <br> &nbsp;&nbsp;&nbsp;&nbsp; money = +prompt('Ваш бюджет на месяц?', '');
> <br> &nbsp;&nbsp;&nbsp;&nbsp; time = prompt('Введите дату в формате YYYY-MM-DD', '2019-06-08');
> <br> }
> <br> start();

<hr>

2. Делаем проверку для **porompt'а** _(внутри function start()...)_

> while(isNaN(money) || money == '' || money == null) {
> <br> &nbsp;&nbsp;&nbsp;&nbsp; money = +prompt('Ваш бюджет на месяц?', '');
> <br> }

<hr>

3. Перемещаем [**наш цикл**](https://github.com/Sadovoy-Danil/Task_2) в новую функцию

> function chooseExpenses() {
> ### &nbsp;&nbsp;&nbsp;&nbsp; Наш цикл
> }
> <br> chooseExpenses();

<hr>

4. Округление переменной _**moneyPerDay**_ до целого числа

> **БЫЛО: appData.moneyPerDay = appData.budget / 30;**

> **СТАЛО: appData.moneyPerDay = (appData.budget / 30).toFixed();**

<hr>

5. Функция для расчета прибыли с депозита за месяц **checkSavings**

> function checkSavings() {
> <br> &nbsp;&nbsp;&nbsp;&nbsp; if (appData.savings == true) {
> <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; let save = +prompt("Какова сумма накоплений?", ""),
> <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; percent = +prompt("Под какой процент?", "");
> <br>
> <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; appData.monthIncome = save / 100 / 12 * percent;
> <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; alert("Доход в месяц с вашего депозита: " + appData.monthIncome);
> <br> &nbsp;&nbsp;&nbsp;&nbsp;}
> <br>}
> <br>
> <br>checkSavings();

<hr>

_**Дополнительное задание**_

- **Оформить расчет дневного бюджета  и вывод на экран этого значения как одну функцию (detectDayBudget)**

> function detectDayBudget() {
> ### &nbsp;&nbsp;&nbsp;&nbsp; [Код](https://github.com/Sadovoy-Danil/Task_2)
> }

<hr>

- **Оформить блок кода с расчетом уровня достатка как отдельную функцию (detectLevel)**

> function detectLevel() {
> ### &nbsp;&nbsp;&nbsp;&nbsp; [Код](https://github.com/Sadovoy-Danil/Task_2)
> }

<hr>

