## Счетчики покрытия JaCoCo
* ### Instructions (C0 Coverage)
Наименьшая единица отсчета JaCoCo - это одиночные инструкции байт-кода Java. Покрытие инструкций предоставляет информацию о количестве кода, который был выполнен или пропущен. Эта метрика полностью независима от исходного форматирования и всегда доступна, даже при отсутствии отладочной информации в файлах классов.
* ### Lines
Для всех файлов классов, скомпилированных с отладочной информацией, можно вычислить информацию о покрытии для отдельных строк. Исходная строка считается выполненной, если была выполнена хотя бы одна команда, назначенная этой строке.
* ### Branches (C1 Coverage)
JaCoCo также вычисляет покрытие ветвей для всех операторов if и switch. Эта метрика подсчитывает общее количество таких ветвей в методе и определяет количество выполненных или пропущенных ветвей. Покрытие ветвей всегда доступно, даже при отсутствии отладочной информации в файлах классов. Обратите внимание, что обработка исключений не рассматривается как ветви в контексте этого определения счетчика.

Выбрала это покрытие, потому что в программе присутствуют операторы for и if.

* ### Cyclomatic Complexity
JaCoCo также вычисляет цикломатическую сложность для каждого неабстрактного метода и суммирует сложность для классов, пакетов и групп. Цикломатическая сложность-это минимальное число путей, которые могут в (линейной) комбинации генерировать все возможные пути с помощью метода. Таким образом, значение сложности может служить показателем количества единичных тестовых случаев для полного охвата определенной части программного обеспечения. Показатели сложности всегда можно рассчитать, даже при отсутствии отладочной информации в файлах классов.
