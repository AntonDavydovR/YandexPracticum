# Анализ пользовательского поведения в мобильном приложении



## Данные

В наличии были следующие данные :

-  EventName — название события; 
-  DeviceIDHash — уникальный идентификатор пользователя; 
-  EventTimestamp — время события; 
-  ExpId — номер эксперимента: 246 и 247 — контрольные группы, а 248 — экспериментальная

## Задача

На основе данных использования мобильного приложения для продажи продуктов питания проанализировать воронку продаж, а также оценить результаты A/A/B-тестирования 

## Используемые библиотеки

- Pandas
- Matplotlib
- Seaborn
- Plotly


## Вывод
1) Мы провели анализ имеющихся данных и определили, что доступный диапазон располагаемой информации находится в промежутке с первого по восьмое августа. В данных наблюдается сильная зависимость от времени суток. В ночное время совершается меньше покупок.
2) Мы выполнили исследование воронки событий. В логах у нас находятся следующие события: появление главного экрана магазина, меню корзины, меню индентификации платежной карты , подтверждение удачной оплаты и меню с инструкцией по пользованию. Каждый пользователь совершал то или иное действие втечение рассматриваемого периода более десяти раз. Это хороший признак, у нас есть постоянная клиентура. Но из общей картины выделяется обучение. Этот пункт не является составляющей воронки, т.к. раздел не обязателен, и не все люди хотят его проходить ( а тем более вновь и вновь возвращаться к нему). Больше всего пользователей ( около 40%) теряется при переходе с главного экрана в корзину. Это логично, т.к. не все готовы совершать покупку. С данным вопросом должны поработать наши маркетологи. Около 20 % пользователей ,перешедших в корзину, теряется на момент оплаты. Это может быть связанно как с тем, что люди в последний момент передумали, так и с технической проблемой. И чуть более 5 % не удается завершить операцию оплаты, что является сугубо техническим вопросом.
3) Мы изучили результаты эксперемента по смене шрифтов. Для успешного проведения A/B-теста мы доказали, что контрольные группы 246 и 247 удовлетворяют условиям A/A-теста (убедились, что различие в количестве пользователей в рассматриваемых группах менее 1%, и что различие ключевых метрик по группам не превышает 1% и не имеет статистической значимости). Далее был проведен ряд A/В-тестов между экспериментальной группой с измененным шрифтом и с двумя контрольными группами. Эти тесты были реализованы в два подхода: сначало с уровнем значимости равным 0.01 ( для уменьшения вероятности появления ошибки первого рода), а затем с уровнем значимости равным 0.1 (для уменьшения вероятности появления ошибки второго рода). Все тесты показали, отрицательный результат. Изменение шрифта в приложении не влияет на количество совершаемых пользователями покупок.


