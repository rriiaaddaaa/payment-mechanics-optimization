# Анализ Результатов A/B Теста Новой Механики Оплаты

## Описание проекта
Этот проект посвящен анализу результатов A/B-тестирования новой механики оплаты на сайте. 

Цель исследования – определить, следует ли запускать новую механику оплаты для всех пользователей, основываясь на ключевых метриках и статистически значимых различиях между целевой и контрольной группами.

## Контекст
В ходе эксперимента одной группе пользователей была предложена новая механика оплаты, в то время как контрольная группа продолжала использовать базовую механику. 
Задача заключалась в оценке влияния новой механики на конверсию, средний доход на пользователя (ARPU) и средний доход на платящего пользователя (ARPPU).

## Структура проекта

1. **Выгрузка данных:** Загрузка данных с Яндекс.Диска.
2. **Обработка данных:** Преобразование данных, создание новых признаков, объединение таблиц, построение и анализ графиков.
3. **Расчет ключевых метрик:** Определение основных метрик для оценки эффективности новой механики.
4. **Статистический анализ:** Проведение статистических тестов для оценки значимости результатов.
5. **Обновление метрик:** Пересчет метрик спустя 2 дня с учетом новых данных о дополнительных пользователях.

## Основные выводы

- **Конверсия (CR):** Снижение конверсии в группе с новой механикой не является статистически значимым, что указывает на отсутствие негативного влияния новой системы оплаты на поведение пользователей.

- **Средний доход (ARPU и ARPPU):** В целевой группе наблюдается значительный рост доходов на пользователя и платящего пользователя, что свидетельствует о положительном влиянии новой механики на общую прибыль.

- **Эффективность и статистическая значимость:** Анализ подтвердил статистически значимые различия в доходах между группами, подтверждая эффективность новой механики оплаты.

  
## Рекомендации
- **Внедрение:** Новую механику оплаты можно внедрить для пользователей, так как она увеличивает доходы без значительного снижения конверсии.
- **Обратный тест:** Провести обратный тест, сохранив старую механику оплаты для 1% пользователей и мониторинг метрик на более длительном сроке для оценки устойчивости эффекта.
- **Оптимизация:** Использовать данные обратного теста для дальнейшей оптимизации системы оплаты, улучшая пользовательский опыт и повышая конверсию.


## Методология

**Анализ данных:**
- **T-тест и U-критерий Манна-Уитни:** Выявили значимость различий в средних доходах.
- **Бутстрап-тестирование:** Подтвердило статистически значимые различия в доходах между группами.
- **Тест Хи-квадрат:** Показал отсутствие статистически значимых изменений в конверсии.

**Инструменты:** Python, Pandas, NumPy, SciPy, Matplotlib, Seaborn.

**Метрики:** Конверсия (CR), средний доход на пользователя (ARPU), средний доход на платящего пользователя (ARPPU).


## Примеры визуализаций
![Alt text](https://github.com/rriiaaddaaa/payment-mechanics-optimization/blob/main/bootstrap.png)

*Пример графика Бутстрап-распределения медиан доходов*


![Alt text](https://github.com/rriiaaddaaa/payment-mechanics-optimization/blob/main/metrics.png)

*Пример графика распределения метрик по группам*

## Описание файла
Файл ab_test_payment_analysis.ipynb содержит подробный анализ данных A/B тестирования, включая код, графики, выводы и рекомендации по запуску новой механики оплаты.
