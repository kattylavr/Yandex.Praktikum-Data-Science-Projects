# **Определение токсичных комментариев для английских текстов**

Интернет-магазин запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию. 

Нужно обучить модель классифицировать комментарии на позитивные и негативные. Для этой задачи создан набор данных с разметкой о токсичности правок.

Нужно построить модель со значением метрики качества *F1* не меньше 0.75. 

**Описание данных**

Данные находятся в файле `toxic_comments.csv`. 

Столбец *text* — текст комментария, а *toxic* — целевой признак.

## **Используемые библиотеки**
pandas, sklearn, numpy, matplotlib, lightgbm, nltk, re, imblearn