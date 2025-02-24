# Домашнее задание к занятию «Разбор типовых ошибок расчётых задач»

## Цель задания

1. Закрепить полученные на лекции знания.
2. Научиться самостоятельно решать задачи оперативного учета из экзамена «1С:Специалист по платформе».

Эта практика позволит вам определить свои сильные и слабые стороны в решении задач оперативного учёта и пригодятся для самостоятельной подготовки к экзамену.

## Чеклист готовности к домашнему заданию

- Просмотреть материал занятия
- Скачать каркасную конфигурацию [файл new_carcass_8_3_17_1496.dt](https://github.com/Bofh82/onec-mid-homeworks/blob/main/OCPS/new_carcass_8_3_17_1496.dt)
- Создать пустую информационную базу
- Загрузить в неё каркасную конфигурацию

## Инструкция к заданию

1. Решите описанную задачу в конфигураторе
2. Протестируйте решение в пользовательском режиме
3. Отправьте на проверку в личном кабинете Нетологии один файл выгрузки базы данных (.dt), содержащий решение задачи. Файл прикрепите в раздел «решение» в практическом задании. Имя файла должно быть в формате «ФамилияИО_СПР4.dt».

## Описание задачи

Начисление зарплаты сотрудникам предприятия осуществляется ежемесячно с использованием метода отклонений. Все начисления могут осуществляться в различных валютах, но учет ведется только в основной валюте. Основная валюта может быть изменена один раз, в начале года. Количество используемых валют заранее неизвестно.

Все сотрудники работают по пятидневному графику, однако необходимо предусмотреть возможность работы по нескольким различным графикам.

Сотрудники получают оплату по окладу пропорционально отработанному времени в днях. Дневная ставка рассчитывается как начальное значение оклада, делённое на количество рабочих дней в том же периоде. В течение расчётного периода оклад не меняется.

Сотрудникам ежемесячно начисляется фиксированная сумма в качестве компенсации проезда к месту работы. Размер суммы в течение расчётного периода не меняется.

Сотрудникам предоставляется оплачиваем отпуск, размер отпускных определяется как количество дней отпуска, умноженное на среднюю дневную ставку. Отпуск считается по календарным дням. 

Средняя дневная ставка определяется как сумма всех начислений на предыдущие 3 месяца, поделенная на количество отработанных дней в трёх предыдущих месяцах. Данные об отпуске могут вводиться в систему задним числом.

Необходимо создать документ «Зарплата к выплате». Документ формируется по конкретному подразделению. В табличной части для каждого сотрудника указывается сумма выплачиваемой зарплаты в валюте учёта. 

Документ должен заполняться автоматически данными о ещё невыплаченной зарплате. На форме документа необходимо предусмотреть кнопку печать, которая формирует ведомость:

Платёжная ведомость №1 за июнь 2023 года по подразделению «Отдел продаж»

| Сотрудник | Вид расчёта | Начальное сальдо | Начислено | К выплате |
|-----------|-------------|------------------|-----------|-----------|
| Петров    |             |100               |300        |360        |
|           |Оклад        |                  |200        |           |
|           |Отпуск       |                  |100        |           |
|           |Выплата      |                  |           |360        |
| Сидоров   |             |                  |500        |500        |
|           |Оклад        |                  |500        |           |
|           |Выплата      |                  |           |500        |
| Итого:    |             |100               |800        |860        |


ОБЯЗАТЕЛЬНО! В пользовательском режиме заведите тестовый пример.

------

### Критерии оценки 

1. Зачёт — реализован весь требуемый функционал, нет критичных ошибок и нарушения логики. Полный перечень ошибок можно найти в [документе на сайте 1С, 3 стр.](https://static.1c.ru/rus/partners/training/files/ATT83PL.rtf?356jhteyner67j340)
2. Введены тестовые данные в пользовательском режиме.
3. На доработку — задание выполнено частично или не выполнено, в логике выполнения заданий есть противоречия, критичные ошибки.
Любые вопросы по решению задач задавайте в чате учебной группы.

*Примерное время выполнения: 45–180 минут*
