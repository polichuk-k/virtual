Задача 1

Опишите кратко, как вы поняли: в чем основное отличие полной (аппаратной) виртуализации, паравиртуализации и виртуализации на 

основе ОС.


Ответ:
Аппаратная виртуализация-гипервизор использует свою хостовую ОС, процессы выполняются с различными приоритетами, гостевые ОС 

получают доступ к ресурсам напрямую

Паравиртуализация-гиперивизору необходимо установленная ОС, гостевые ОС используют собственные ресурсы выделенные гипервизором

Виртуализация на основе ОС -роль гипервизора берет ядро хостовой ОС, разделение ресурсов а также гостевые ос легковесные


Задача 2

Выберите один из вариантов использования организации физических серверов, в зависимости от условий использования.

Организация серверов:

    физические сервера,
    паравиртуализация,
    виртуализация уровня ОС.

Условия использования:

    Высоконагруженная база данных, чувствительная к отказу.
    Различные web-приложения.
    Windows системы для использования бухгалтерским отделом.
    Системы, выполняющие высокопроизводительные расчеты на GPU.

Опишите, почему вы выбрали к каждому целевому использованию такую организацию.


физические сервера- Системы, выполняющие высокопроизводительные расчеты на GPU,  Высоконагруженная база данных, Windows системы 

для использования бухгалтерским отделом.чувствительная к отказу.
Так как данные системы требуют больших вычислительных ресурсов и высокой надежности
    
паравиртуализация- Windows системы для использования бухгалтерским отделом.
Не требуются высокие мощности, также можно увиичивать ресурсы гостевых ос

виртуализация уровня ОС- Различные web-приложения.
Так как работа web прилжений требует мало ресурсов и для каждого приложения лучше использовать свою среду и миграция контейнеров 

происходит намного быстрее.



Задача 3

Выберите подходящую систему управления виртуализацией для предложенного сценария. Детально опишите ваш выбор.

Сценарии:

100 виртуальных машин на базе Linux и Windows, общие задачи, нет особых требований. Преимущественно Windows based инфраструктура, 

требуется реализация программных балансировщиков нагрузки, репликации данных и автоматизированного механизма создания резервных 

копий.

Аппаратная виртуализация, например esxi vmware, удобно работать, большие возможности

Требуется наиболее производительное бесплатное open source решение для виртуализации небольшой (20-30 серверов) инфраструктуры на 

базе Linux и Windows виртуальных машин.

Паравиртуализация например, например kvm так как бесплатная лицензия

Необходимо бесплатное, максимально совместимое и производительное решение для виртуализации Windows инфраструктуры.

Паравиртуализация, например hyper-v, идет в составе компонентах windows

Необходимо рабочее окружение для тестирования программного продукта на нескольких дистрибутивах Linux.

Паравиртуализация, например virtual box или wmware


Задача 4

Опишите возможные проблемы и недостатки гетерогенной среды виртуализации (использования нескольких систем управления 

виртуализацией одновременно) и что необходимо сделать для минимизации этих рисков и проблем. Если бы у вас был выбор, то 

создавали бы вы гетерогенную среду или нет? Мотивируйте ваш ответ примерами.

В гетерогенных средах, когда приложения размещены в разных средах виртуализации, каждой такой средой приходится управлять 

собственным инструментом. Общей консоли на данный момент на рынке не существует, и пока имеется только один выход — механизм 

скриптов, что довольно сложно, трудоемко и может значительно усложнить задачи управления и мониторинга. Если был бы выбор, то не 

создавал бы подобную среду, так как в средних и мелких компаниях этого не требуется.
