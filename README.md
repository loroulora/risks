# risks
## My project analysis dedicated to the risks of issuing a mortgage in the banking system


## Компания занимается ипотечный кредитованием. Вы работаете в отделе рисков. Ваши основные задачи:

  1.	Обеспечить уровень просрочки по выдаваемым кредитам в 1% (1 кредит из 100 будет просрочен);

  2.	Максимизировать уровень одобрения по заявкам на кредит.

### Ваш руководитель выдвинул гипотезу, что отношение первоначального взноса к стоимости недвижимости (ПВ) хорошо ранжирует платёжеспособность клиентов (уровень просрочки).

### Вам необходимо:

  1.	Проверить гипотезу и составить аналитическую записку (ретро данные в файле «dataset.csv»);

  2.	Составить предложение по использованию ПВ в Системе Принятия Решения (СПР –автоматизированный набор методов проверки платежеспособности   клиента, результатом работы которого является заключение: одобрить/отказать);

   3.	Оценить эффект на уровень одобрения от внедрения вашего инициативы (данные по актуальным заявкам в папке «БД»);

  4.	Составить бизнес-требование для разработчиков, на основании которого будет реализовано ваше предложение;

  5.	Описать тестовые кейсы, на основании которых будет проведена проверка корректности технической реализации вашего предложения.

### Описание данных

### Поля из файла «dataset.csv»:

  1.	application_id – идентификатор заявки;

  2.	pd – оценка вероятности просрочки (Probability of Default) – один из основных инструментов управления уровнем просрочки по кредитному 
  портфелю;

  3.	initinal_payment – первоначальный взнос/стоимость недвижимости (ПВ);

  4.	delay – флаг просрочки (1 – просрочен, 0 – не просрочен).

БД – набор CSV файлов, которые имитируют базу данных (БД). В ходе работы СПР в БД записываются данные по обработке заявки.

### Требования по выполнению задания

  1.	Анализировать данные можно, используя любые инструменты (excel, python, и т.д.); 

  2.	При работе с файлами из папки «БД» напишите SQL скрипт/скрипты под каждую манипуляцию с данными, которая потребуется для решения задачи. 

Например, для решения задачи необходимо посчитать количество заявок по источникам:

«select source, count(*) as cnt_apps from spr_application group by source»

