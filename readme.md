Описание алгоритма

Предполагается, что на вход подаются заведомо коректные значения диапозонов [нижняя граница, верхняя граница]

В начале происходит проверка значений заданного диапозона, если оба значения равны null возвращаем все курсы, тк границы не установлены
Далее фильтрация курсов если нижняя граница заданного диапозона равна null, 
Условия для фильтрации: нижняя граница цены курса не установленна или меньше или равна верхней границе диапозона
Далее фильтрация курсов если нижняя границы заданного диапозона равна null
Условия для фильтрации:  верхняя граница цены курса не установленна или больше или равна нижней границе диапозона
Далее фильтрация по умолчанию если обе границы диапозона установленны
Условия для фильтрации:
Если обе границы курса не установленны, возвращаем этот курс, тк он подходит под любой диапозон
Если нижняя граница курса не установленна и верхняя граница больше или равна нижней границе диапозона, возвращаем этот курс
Если верхняя граница курса не установленна и нижняя граница меньше или равна верхней границе диапозона, возвращаем этот курс
Ecли все значения границ курсов и диапозона установленны проверяем что любая из границ цены курса входит в диапозон или границы цен курса меньше и больше соответствующих значениц диапозона, возвращаем этот курс  

