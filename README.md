# Task_INT20H

## Инструкция:

1. Загрузить Jupyter Notebook 
1. Клонировать репозиторий 
1. Открыть Task_INT20H.ipynb

## Результат LTV = 9517.473

----

**Task 2 (Analytical)**. Ви - аналітик в стартапі, вам потрібно допомогти <br>
маркетинговій команді розрахувати ключові показники. Ваш стартап - додаток<br>
у якого модель монетизації є підписка. Спочатку юзер бере тріал (він триває 7<br>
днів), після кінця тріалу він може відписатись, або ж продовжити платити за<br>
тижневу підписку. Підписка коштує 9.99 за тиждень. Юзер може відписатись у<br>
будь-який момент, після цього він не буде більше платити.<br>

Ваше завдання - розрахувати LTV за допомогою Python. Будемо оцінювати<br>
ваше загальне розуміння завдання та результат. У файлі data_analytics.csv ви<br>
знайдете фрагмент бази даних, що вам потрібна, де:<br>

Event Date – дата коли відбулась подія (тріал чи продовження підписки).<br>

Subscription Offer Type – тип підписки (якщо вказано Free Trial - значить це<br>
початок тріалу, якщо поле пусте - це підписка).<br>

LTV – lifetime value. У цьому випадку рахується через конверсії з тріалу в<br>
оплату і потім в наступні оплати. <br>

LTV = ([1]+[2]+[3]+[4]+[5]), де [1] = (dev proceeds * Conversion to trial), а [2] = [1] * 1st
purchase to 2nd, [3] = [2] * 2nd to 3rd і тд.<br>

