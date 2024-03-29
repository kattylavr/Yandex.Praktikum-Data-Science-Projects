# **Определение выгодного тарифа для телеком компании**
## **Данные**
Таблица users — информация о пользователях:<br>
- user_id — уникальный идентификатор пользователя<br>
- first_name — имя пользователя<br>
- last_name — фамилия пользователя<br>
- age — возраст пользователя (годы)<br>
- reg_date — дата подключения тарифа (день, месяц, год)<br>
- churn_date — дата прекращения пользования тарифом (если значение пропущено, значит, тариф ещё действовал на момент выгрузки данных)<br>
- city — город проживания пользователя<br>
- tarif — название тарифного плана<br>

Таблица calls — информация о звонках:<br>
- id — уникальный номер звонка<br>
- call_date — дата звонка<br>
- duration — длительность звонка в минутах<br>
- user_id — идентификатор пользователя, сделавшего звонок<br>

Таблица messages — информация о сообщениях:<br>
- id — уникальный номер звонка<br>
- message_date — дата сообщения<br>
- user_id — идентификатор пользователя, отправившего сообщение<br>

Таблица internet — информация об интернет-сессиях:<br>
- id — уникальный номер сессии<br>
- mb_used — объём потраченного за сессию интернет-трафика (в мегабайтах)<br>
- session_date — дата интернет-сессии<br>
- user_id — идентификатор пользователя<br>

Таблица tariffs — информация о тарифах:<br>
- tariff_name — название тарифа<br>
- rub_monthly_fee — ежемесячная абонентская плата в рублях<br>
- minutes_included — количество минут разговора в месяц, включённых в абонентскую плату<br>
- messages_included — количество сообщений в месяц, включённых в абонентскую плату<br>
- mb_per_month_included — объём интернет-трафика, включённого в абонентскую плату (в мегабайтах)<br>
- rub_per_minute — стоимость минуты разговора сверх тарифного пакета (например, если в тарифе 100 минут разговора в месяц, то со 101 минуты будет взиматься плата)<br>
- rub_per_message — стоимость отправки сообщения сверх тарифного пакета<br>
- rub_per_gb — стоимость дополнительного гигабайта интернет-трафика сверх тарифного пакета (1 гигабайт = 1024 мегабайта)<br>

## **Задача**

Проанализировать поведение клиентов и сделать вывод — какой тариф лучше. Проверить две гипотезы о выручке пользователей.

## **Используемые библиотеки**
pandas, numpy, seaborn, matplotlib, scipy, os