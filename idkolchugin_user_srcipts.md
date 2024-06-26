# Кольчугин Иван - "Boolify"
# Пользовательские сценарии

### Группа: 10 - И - 4
### Электронная почта: ivankolcugin@gmail.com
### Telegram: [@tertemiss](https://t.me/tertemiss)


### [ Сценарий 1 - Ввод булевых выражений]

1. Главное окно подразделяется на два основных: экранная клавиатура с различными операциями для работы с булевой алгеброй и окно, где отображется набранное пользователем выражение, результат вычислений.
2. Пользователь набирает на экранной клавиатуре либо булеву функцию, что необходимо упростить, либо булево уравнение, что необходимо решить.
3. Если введена булева функция, что необходимо упростить, в окне вывода показывается упрощенная функция.
4. Отдельно пользователь может запросить вывод пошагового упрощения, ДНФ, КНФ, СДНФ, СКНФ, таблицы истинности.
5. Если введено булево уравнение, в окне вывода, в виде таблицы показываются все возможные комбинации переменных (влияющих на результат), приводящие к решению уравнения.
6. Если все возможные комбинации переменных не помещаются на экране, они выводятся лишь частично (в виде выпадающего списка), вторая часть выводится при его раскрытии.
7. Отдельно пользователь может запросить вывод пошагового решения уравнения, полной таблицы истинности.

### [ Сценарий 2 - Просмотр истории введенных выражений]

1. Пользователь в меню выбирает раздел истории введенных выражений.
2. Перед пользователем появляется лента ранее сохраненных им выражений.
3. Если пользователь не сохранял ранее функции или уравнения, то появляется сообщение о том, что записи о упрощенных функциях/решенных уравнениях отсутствуют.
4. Пользователь может выбрать одно из ранее введенных им выражений.
5. Если выбранное выражение - функция, пользователь может видоизменить данную функцию или запросить вывод пошагового упрощения, ДНФ, КНФ, СДНФ, СКНФ, таблицы истинности, упрощенной функции.
6. Если выбранное выражение - уравнение, пользователь может видоизменить данное уравнение или запросить вывод пошагового решения уравнения, всех возможных комбинаций переменных, приводящих к решению уравнения.
7. Если пользователь выбирает видоизменение выражения, то он переходит в раздел ввода булевых выражений к сценарию 1.

### [ Сценарий 3 - Настройка работы приложения]

1. Пользователь в меню выбирает раздел настроек работы приложения.
2. Перед пользователем появляется список доступных настроек: очищение истории введенных выражений, выбор темной/светлой темы, смена графического представления операций.
3. Если пользователь выбирает очищение истории введенных выражений, база данных удаляет записи о введенных пользователем выражениях.
4. Если пользователь выбирает смену темы, то ему на выбор предлагается темная/светлая цветовая гамма.
5. При смене темы на на темную/светлую, цветовая гамма приложения меняется на соответствующую.
6. Если пользователь выбирает смену графического представления операции, появляется окно с возможностью изменения графического представления операции, на выбор, из возможных (от двух до трех).
7. При выборе нового графического представления операции, ее изображение во всех местах, где она позиционирует, изменяется на соответствующее (на экранной клавиатуре, в истории введенных выражений, в меню выполнения вычислений и т.п.)

### [ Сценарий 4 - Упрощение булевых функций]

1. Пользователь, в сценарии 1, вводит булеву функцию, что необходимо упростить.
2. Если функция уже имеет свой наиболее упрощенный вид, то программа сообщает об этом пользователю.
3. Если введенная функция некорректна (например, отсутсвуют открыващие/закрывающие скобки, операции между переменными и т.д.), выводится сообщение о том, что введенная функция некорректна.
4. В окне вывода выводится минимально возможная упрощенная форма функции.
5. При запросе пользователя (нажатия на иконку сохранения), данная функция записывается в историю введенных выржений.
6. Отдельно пользователь может запросить вывод СКНФ, СДНФ, ДНФ, КНФ, таблицы истинности, пошагового упрощения функции.
7. Если пользователь запрашивает вывод СКНФ, СДНФ, ДНФ, КНФ, таблицы истинности, то он переходит к сценарию 6
8. Если пользователь запрашивает пошаговое упрощение функции, он переходит к сценарию 7.

### [ Сценарий 5 - Решение булевых уравнений]

1. Пользователь, в сценарии 1, вводит булево уравнение, что необходимо решить.
2. Если у уравнения нет решений или оно всегда тождественно, то программа сообщает об этом пользователю.
3. Если уравнение некорректно (отсутсвуют открыващие/закрывающие скобки, пустое поле с одной из сторон уравнения и т.д.) программа сообщает, что данное уравнение некорректно.
4. В окне вывода выводится таблица истинности с переменными, что приводят к решению уравнения и влияют на его результат.
5. При нажатии на иконку сохранения, введенное уравнение сохраняется в историю введенных выражений.
6. Отдельно пользователь может запросить вывод полной таблицы истинности (со всеми переменными, в т. ч. не влияющими на результат), пошагового решения уравнения.
7. Если пользователь запрашивает вывод полной таблицы истинности, то он переходит к сценарию 6
8. Если пользователь запрашивает пошаговое упрощение уравнения, то он переходит к сценарию 7.

### [ Сценарий 6 - Вывод СКНФ, СДНФ, КНФ, ДНФ, таблицы истинности]

1. Пользователь запрашивает вывод СКНФ/СДНФ/КНФ/ДНФ, 
2. Перед пользователем возникает список с каждым из этих представлений выражения
3. При необходимости пояснения получения какой-либо из этих форм пользователь нажимает на нее.
4. Перед пользователем раскрывается список шагов, приводящих функцию к данному представлению.
5. Пользователь запрашивает вывод таблицы истинности выражения.
6. Перед пользователем появляется полная таблица истинности выражения N + 1 (все переменные и результат выражения) столбцов и N^2 + 1 (заглавие и все комбинации переменных) строк, где N - кол-во переменных.
7. Если таблица истинности не полностью помещается на экране устройства, она появится лишь частично и раскроется полностью только при нажатии на нее.

### [ Сценарий 7 - Вывод пошагового упрощения функции/уравнения]

1. Пользователь запрашивает пошаговое упрощение функции/уравнения.
2. Если данное выражение по каким-то причинам невозможно упростить (некорректная запись и т.п.), пользователю выводится сообщение об этом.
3. Если выражение уже имеет минимальную форму, то пользователю выводится сообщение об этом.
4. Перед пользователем появляется список шагов, что приводит выражение к его минимально возможному виду.
5. При нажатии на какой-либо из шагов открывается пояснение, объясняющее прием, использованный для упрощения выражения.
6. При повторном нажатии на шаг с раскрытым объяснением, оно скрывается обратно.
7. При нажатии кнопки возврата пользователь возвращается к сценарию 1.
