# PPvIS_lab3_Graph

Тема: Создание пользовательских элементов управления. Многопоточная обработка.

Написать приложение, которое рисует график вычисления функции из варианта задания. В левой части окна должна располагаться таблица вычисленных значений функции.

Рисование графика должно происходить на пользовательском виджете (подклассе
QWidget с перегруженным методом paintEvent). Должны рисоваться оси координат с
подписями на стрелках. Также подписями должны быть отмечены начало координат и
деления на осях. Если график не помещается на виджет, то должны появляться
вертикальные и горизонтальные полосы прокрутки. При зажатой на графике только левой
клавише мыши и ее перетягивании должен происходить сдвиг отображаемой области
графика. Если зажать клавишу Ctrl и крутить колѐсико мыши на графике, то должно
произойти масштабирование (увеличение/уменьшение размеров).
Под виджетом графика должна располагаться группа элементов, которая показывает
текущий режим отображения графика и позволяет задавать параметры для вычисления
таблицы функции. Содержимое этой группы элементов зависит от варианта, но всегда
должны быть элемент отображения кратности масштабирования и кнопка «Построить
график», при нажатии на которую происходит построение графика. Программа должна
сообщать пользователю о введение некорректных параметров вычисления функции.
При выполнении вариантов, которые предусматривают работу с файлами,
необходимо использовать классы ввода/вывода библиотеки Qt.

В этой лабораторной работе необходимо будет вынести вычисление значений функции в отдельный поток (создать подкласс QThread, который будет осуществлять вычисление). Для синхронизации потоков можно использовать на выбор преподавателя только QMutex, QReadWriteLock, QSemaphore, QWaitCondition и нельзя использовать сигналы-слоты.

Вариант 15

Таблица функции задается по следующему правилу: на вход программе подается
текстовый файл. Программа генерирует случайные строки от 1 до n элементов, затем
начинает искать вхождения каждой сгенерированной строки в файле поданном на вход. В
таблицу заносятся время поиска каждой строки и количество символов. Построить
зависимость времени поиска от количества символов используя алгоритм прямого поиска
строки.