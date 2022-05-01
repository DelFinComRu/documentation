# Документация к системе ДелФин (https://delfin.com.ru)


Чтобы получить оптимальное соотношение функциональных возможностей и финансовых затрат, необходимо на этапе проектирования инфраструктуры изучить правила лицензирования и выбрать подходящие редакции ОС и СУБД.
При выборе редакции учитывайте:
- версию ОС и СУБД;
- количество ядер процессора;
- количество развернутых виртуальных машин;
- поддержку отказоустойчивых кластеров.


# Аппаратные требования 
Аппаратные требования к компьютеру с серверной частью (серверу СУБД) зависят от количества одновременно работающих пользователей системы, которых может быть в несколько раз меньше общего числа зарегистрированных пользователей.

Минимальные системные требования для одновременной работы 10 пользователей:
Linux Debian 8+
CPU 2 Core 2.00 Mgz
RAM 2 GB
HDD/SSD 128 GB

#Создание документов

Документ - сущность в системе документооборота которая может быт классифицирована по типу и классу.

Классы - документов основные ответвления (входящие, исходящие, внутренние).

Типы документов - служебная записка, письмо, акт и т.д.

На каждой странице ЭДО доступа кнопка «Создать документ». 

Свойства документа:

1. Краткое описание документа
Текстовое поле.  Используется для краткого описания документа. Свойство фигурирует на странице поиска документов. Должно отражать тему документа.

2. Класс документа
Выбор из списка. Классификатор документа (внутренний, исходящий, входящий).

3. Контрагент
Выбор из списка с автодополнением и автосозданием. Позволяет связать документ с с элементом из справочника «Контрагент». Возможен ввод по ИНН.

4. Адрес
Выбор из списка с автодополнением и автосозданием. Позволяет связать документ с с элементом из справочника «Адрес». 

5. Тип
Выбор из списка с автодополнением. Свойство указывает на тип документа. Может быть дополнен на этапе внедрения.

6. Статус
Выбор из списка с автодополнением.  Свойство указывающий на текущий статус документа.

7. Срок документа
Выбор из формы календаря. Свойство указывающее на срок в который документ должен быть обработан (изменён статус на «Отработан»). По этому полю происходить формирование календаря. 

8. Содержимое.
Текстовая область. Полное содержимое документа. По этому полю происходит поиск типа «по содержанию».  Длина поля не ограничена. 

9. Связующий документ.
Выбор из списка с автодополнением.  Позволяет установить связь создаваемого документа по номеру с другими документами в ЭДО.

10. Файлы во вложении
Область загрузки файлов. Позволяет загрузить к доументу дополнительные файлы графического и текстового формата.  Документы будут хранится в экземпляре ЭДО.

Назначение документа:

Маршрут по умолчанию для новых документов имеет «вертикальный» маршрут движения. При указании департамента назначения после достижения конечной точки в вертикальном движении (по организационной структуре предприятия) документ будет перемещён в департамент указанный в этом поле. 
При указании конкретного сотрудника (поле «Сотрудник») документ будет перемещён в область видимости указанного сотрудника.




