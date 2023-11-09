# Портфолио: аналитик данных
## Обо мне 
Привет! Меня зовут Анна, я начинающий аналитик данных. В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения и практики.

## Навыки и технологии 
- Инструменты анализа данных: ***SQL, Excel***
- Языки программирования и библиотеки: ***Python, Pandas, math***
- Системы управления базами данных: ***PostgreSQL***
- Средства визуализации данных:  ***Matplotlib, seaborn***
  
# Проекты

## **Проект 1: Калькулятор юнит-экономики онлайн-кинотеатра**

### **Задачи:**
1. Собрать калькулятор юнит-экономики продукта
2. Посчитать юнит-экономику продукта и предложить сценарий по настройке параметров для выхода на 25%-ную маржинальность
3. Собрать визуализации основных бизнес-показателей
4. Исследовать данные о пользователях и их поведении.

> [Проект 1](https://github.com/PanshinaAnna/portfolio/blob/f492b54805cf6cee7d26da21f394c49fbe674b23/%D0%9A%D0%B0%D0%BB%D1%8C%D0%BA%D1%83%D0%BB%D1%8F%D1%82%D0%BE%D1%80%20%D1%8E%D0%BD%D0%B8%D1%82-%D1%8D%D0%BA%D0%BE%D0%BD%D0%BE%D0%BC%D0%B8%D0%BA%D0%B8%20%D0%BE%D0%BD%D0%BB%D0%B0%D0%B9%D0%BD-%D0%BA%D0%B8%D0%BD%D0%BE%D1%82%D0%B5%D0%B0%D1%82%D1%80%D0%B0.xlsx)

**Итоги:**

1. Собран функционирующий калькулятор юнит-экономики. 
2. Рассчитана юнит-экономика продукта. Из динамики роста пользователей и выручки следует, что что приток новых пользователей существенно сократился.
3. Активность пользователей оформлена в виде гистограмм. 

## **Проект 2: Построение витрины для модели машинного обучения в банке**

### **Задача:**
Составить витрину для модели специалистов по машинному обучению

**Краткое описание решения задач:**

> [Проект 2](https://github.com/PanshinaAnna/portfolio/commit/b17373c5ea6480f06d23019dc390ebf8a9a72b11)
> 
> На основании таблицы *skybank.late_collection_clients* пишу запрос. С помощью оконных функций добавляю поля, где отображается:
>  - Суммарный объем кредитов, доля данного кредита среди всех кредитов выданных и количество кредитов в этом городе.
>  - Суммарный объем кредитов, доля данного кредита среди всех кредитов выданных и количество кредитов в рамках указанного типа кредита.
>  - Суммарный объем кредитов, доля данного кредита среди всех кредитов выданных и количество кредитов в рамках указанного типа кредита и города.

**Итог** 

Результат запроса - витрина для модели машинного обучения в банке. 


## **Проект 3: Моделирование изменения балансов студентов**

### **Задачи:**
1.  Смоделировать изменение балансов студентов
2.  Визуализировать итоговоговый результат

**Краткое описание решения задач:**

> [Проект 3](https://github.com/PanshinaAnna/portfolio/commit/879ef1963f85945efb2c93576b1ec8539f2238ef)
> 
> Для начала определила, когда была первая транзакция для каждого студента. С этой даты собираю его баланс уроков. Собрала таблицу с датами за каждый календарный день года. Далее узнаю, за какие даты имеет смысл собирать баланс для каждого студента.
> Для этого объединяю таблицы и создаю CTE *all_dates_by_user*, где будут храниться все даты жизни студента после того, как произошла его первая транзакция.
> Нашла все изменения балансов, связанные с успешными транзакциями. Для этого объединяю *all_dates_by_user* и *payments_by_dates* по дате и id студента.
> Определила баланс студентов, который сформирован только транзакциями. Создаю CTE *classes_by_dates*, где считаю количество уроков за каждый день для каждого ученика.
> Создаю CTE для количества пройденных уроков. Для этого объединяю таблицы *all_dates_by_user* и *classes_by_dates* по дате и id студента.
> Создаю CTE *balances* с вычисленными балансами каждого студента.
> Суммирую поля и смотрю, как менялось общее количество уроков на балансах студентов.
> Визуализирую и делаю выводы. 

**Итоги:**

1. Результатом проекта является запрос, который собирает данные о балансах студентов за каждый прожитый ими день. На их основании можно проанализировать и сделать выводы о работе школы за год. 
2. Графики показывают хорошую динамику за год. Количество купленных уроков растет, школа развивается 

# Контакты:
- Email: anna.vl21@yandex.ru
