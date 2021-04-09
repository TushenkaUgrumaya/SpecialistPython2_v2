## ТЗ “I-Bank” Часть-1

## Цель

Разработать класс для консольного приложения “I-Bank” для хранения денежных вкладов и манипуляций с ними.


### Возможности класса

1. Создавать новый счет для клиента
1. Посмотреть счет по номеру паспорта клиента
1. Узнать состояние счета
1. Положить деньги на счет
1. Снять деньги со счета
1. Перевести деньги на счет другому клиенту


### Подробнее о счете

При создании нового счета необходимо указать информацию:

*   Имя клиента
*   8-ми значный номер паспорта
*   Номер телефона клиента в формате (+7-9xx-xxx-xx-xx)

Номер паспорта является ключом доступа к счету. Т.е. пользователь должен указать номер паспорта, чтобы иметь возможность выполнять операции со своим счетом.

Номер телефона служит для перевода от других клиентов данному клиенту.


#### “Создать новый счет”

Запрашивает данные о клиенте и создает новый объект счета

**_Опционально_**: Проверяет, что номер паспорта и номер телефона являются уникальными.


#### “Посмотреть счет по номеру паспорта”

Запрашивает номер паспорта клиента и отображает его счет(в формате):

Иван баланс: 21283 руб. телефон:+7-912-622-11-22

#### “Узнать состояние своего счета”

Отображает баланс счета, формат выберите самостоятельно

#### “Положить деньги на счет”

Клиент указывает сумму и она добавляется к его текущему счету. Считается, что мы симулируем ситуацию перевода средств, например,с банкомата или через кассу банка.


#### “Снять деньги со счета”

Клиент указывает сумму и если на его счету достаточно средств, то сумма списывается со счета. Если денег на счету недостаточно, то выдается соответствующее предупреждение. Пока считаем, что клиент не может работать с банком в кредит и его счет всегда должен оставаться положительным.


#### “Перевести деньги на счет другому клиенту”

Программа запрашивает номер телефона, если клиент с таким номером найден, то просит указать переводимую сумму. Сумма списывается с одного счета и зачисляется на другой.

Также требуется проверить наличие переводимой суммы.