# YandexPracticum
Данные проекты были выполнены в ходе обучения в Яндекс.Практикуме, профессии "Аналитик данных".

| Название проекта | Описание | Используемые библиотеки и инструменты | 
| :---------------------- | :---------------------- | :---------------------- |
| 1. [Исследование надёжности заёмщиков — анализ банковских данных] (Исследование надёжности заёмщиков — анализ банковских данных) | На основе данных кредитного отдела банка исследовал влияние семейного положения и количества детей на факт погашения кредита в срок. Была получена информация оанных. Определены и обработаны пропуски. Заменены типы данных на соответствующие хранящимся данным. Удалены категоризированны данные. Удалены дубликаты. Выделены леммы в значениях столбца и категоризированны данные. | предобработка данных, Python, Pandas, PyMystem3, лемматизация|
| 2. Продажа квартир в Санкт-Петербурге — анализ рынка недвижимости | На основе данных сервиса Яндекс.Недвижимость определена рыночная стоимость объектов недвижимости разного типа, типичные параметры квартир, в зависимости от удаленности от центра. Проведена предобработка данных. Добавлены новые данные.Построены гистограммы,боксплоты, диаграммы рассеивания. | Python, Pandas, Matplotlib, исследовательский анализ данных, визуализация данных, предобработка данных |
| 3. Определение выгодного тарифа для телеком компании | Проведен предварительный анализ использования тарифов на выборке клиентов,проанализировано поведение клиентов при использовании услуг оператора и рекомендованы оптимальные наборы услуг для пользователей. Проведена предобработка данных, их анализ. Проверены гипотезы о различии выручки абонентов разных тарифов и различии выручки абонентов из Москвы и других регионов. | Python, Pandas, Matplotlib, NumPy, SciPy, описательная статистика, проверка статистических гипотез|
| 4. Изучение закономерностей, определяющих успешность игр| Выявлены параметры, определяющие успешность игры в разных регионах мира. На основании этого подготовлен отчет для магазина компьютерных игр для планирования рекламных кампаний. Проведена предобработка данных, анализ. Выбран актуальный период для анализа. Составлены портреты пользователей каждого региона. Проверены гипотезы: средние пользовательские рейтинги платформ Xbox One и PC одинаковые; средние пользовательские рейтинги жанров Action и Sports разные. При анализе использовал критерий Стьюдента для независимых выборок. |Python, Pandas, NumPy, Matplotlib, предобработка данных, исследовательский анализ данных, описательная статистика, проверка статистических гипотез|
| 5. Исследование данных авиакомпании — проверить гипотезу о повышении спроса во время фестивалей| Проведена выгрузка и подготовка предоставленных данных авиакомпании средствами SQL. Проверена гипотеза о различии среднего спроса на билеты во время проведения различных фестивалей и в обычное время . |SQL, Python, Pandas, Matplotlib, SciPy, проверка статистических гипотез|
| 6. Оптимизация маркетинговых затрат в Яндекс.Афише| Проведен анализ данных от Яндекс.Афиши целью оптимизации маркетинговых затрат.Рассчитаны метрики LTV, CAC, Retention rate, DAU, WAU, MAU, ROMI|Python, Pandas, Matplotlib, когортный анализ, юнит-экономика, продуктовые метрики|
| 7. Проверка гипотез по увеличению выручки в интернет-магазине —оценить результаты A/B теста| Проведена приоритизация гипотез по фреймворкам ICE и RICE. Затем провел анализ результатов A/B-теста, построил графики кумулятивной выручки, среднего чека,конверсии по группам, а затем посчитал статистическую значимость различий конверсий  средних чеков по сырым и очищенным данным. На основании анализа мной было принято решение о нецелесообразности дальнейшего проведения теста.|Python, Pandas, Matplotlib, SciPy, A/B-тестирование, проверка статистических гипотез|
| 8. Исследования рынка общепита в Москве для принятия решения об открытии нового заведения| Мною был исследован вопрос - будет ли успешным и популярным на долгое время кафе, в котором гостей обслуживают роботы-официанты. По результатам анализа подготовлена презентация для инвесторов с рекомендациями. В построении графиков я использовали библиотеки seaborn и plotly. Также мне потребовалось получить район расположения кафе-конкурентов. Эту задачу я решил, подключившись к API Яндекс.Геокодер библиотекой requests|Python, Pandas, Seaborn, Plotly, визуализация данных|
| 9. Анализ пользовательского поведения в мобильном приложении| В данном проекте мной были изучены принципы событийной аналитики. Я построил воронку продаж, исследовал путь пользователей до покупки. Проанализировал результаты A/B-теста введения новых шрифтов. Сравнил 2 контрольных группы между собой, убедился в правильном разделении трафика, а затем сравнил с тестовой группой Выявлено, что новый шрифт значительно не повлияет на поведение пользователей.|A/B-тестирование, Python, Pandas, Matplotlib, Seaborn, событийная аналитика, продуктовые метрики, Plotly, проверка статистических гипотез, визуализация данных|
| 10. Создание дашборда по пользовательским событиям для агрегаторановостей| Работу над этим проектом я провел на удаленной машине в сервисе Yandex.Cloud. Мной был установлен PostgreSQL, развернута база данных. Затем я написал скрипт пайплайна, который позволил собирать данные за определенный временной период, и настроил его автономную работу через crontab. Для визуализации собранных данных я написал скрипт дашборда с несколькими фильтрами и также запустил его на удаленной машине. По результатам была подготовлена презентация с полученными графиками|Python, SQLAlchemy, PostgreSQL, dash, Tableau, продуктовые метрики, построение дашбордов|
| 11. Прогнозирование вероятности оттока пользователей для фитнес-центров| В данном проекте использовано машинное обучение. Спрогнозирована вероятность оттока (на уровне следующего месяца) для каждого клиента; сформированы типичные портреты пользователей: выделены наиболее яркие группы, охарактеризованы их основные свойства; проанализированы основные признаки, наиболее сильно влияющиена отток.|Python, Pandas, Scikit-learn, Matplotlib, Seaborn, машинное обучение, классификация, кластеризация|








