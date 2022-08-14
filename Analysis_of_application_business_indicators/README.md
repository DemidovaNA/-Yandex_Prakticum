# Тема: Анализ бизнес-показателей

# Проект: Анализ бизнес-показателей развлекательного приложения

#### Описание проекта 
На протяжении последних нескольких месяцев бизнес несет убытки. В привлечение пользователей вложено много денег, а результата нет. Необходимо разобраться в причинах этой ситуации.

##### Исходные данные:

* лог сервера с данными о посещениях приложения новыми пользователями, зарегистрировавшимися в период с 2019-05-01 по 2019-10-27;
* выгрузка покупок пользователей за этот период;
* статистика рекламных расходов.

##### Цель - ответить на вопросы:

* как люди пользуются продуктом;
* когда они начинают покупать;
* сколько денег приносит каждый клиент;
* когда он окупается и какие факторы отрицательно влияют на привлечение пользователей.

#### Навыки и инструменты использованные в проекте:
* Python, Pandas, Matplotlib, Seaborn, NumPy, когортный анализ, юнит-экономика, продуктовые метрики.



#### Краткие выводы
##### Причины неэффективности привлечения пользователей:

* На общую картину неэффективности привлечения повлияли пользователи из региона США. Их количество больше половины от всего объема привлеченных пользователей, а показатель САС неуклонно рос на протяжении всего периода исследования.
* Вероятно, что основным поставщиком трафика из региона США является платформа TipTop. Об этом косвенно свидетельствует растущий график "динамики стоимости привлечения пользователей" в пункте 5.3 и 5.4. Расходы на привлечение пользователей из данного канала составляют 51,8% от общего объема затрат.
* Возможно причиной подобного объема затрат на платформе TipTop стал некорректный выбор модели оплаты рекламы.
* На основе графика удержания платящих пользователей можно предположить, что качество привлеченной аудитории с платформ FaceBoom и AdNonSense низкое. Это влияет на показатель удержания, что в свою очередь влияет на LTV, а оно влияет на ROI.
* Возможно при адаптации приложения под IOS разработчики и дизайнеры не следовали стандартам платформы и как следствие приложение нестабильно или им неудобно пользоваться. Данный аспект повлиял на удержание пользователей с устройствами Mac и iPhone.

##### Рекомендации для отдела маркетинга для повышения эффективности:

* Оптимизировать бюджет для платформы TipTop. Возможная смена модели покупки трафика.

* Релокация части бюджета на платформы с доказанной эффективностью. Например: WahooNetBanner, RocketSuperAds, lambdaMediaAds.

* Провести А/В тестирование рекламных сообщений для увеличения охвата на эффективных площадках.

* Добавить в развлекательное приложение полезный функционал. Это увеличит ценность продукта и как следствие повысит показатели удержания.