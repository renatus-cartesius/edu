# 1. Введение в предмет, основные понятия и термины.
##  Основные понятия.

Исходное представление о базах данных массового пользователя будет, скорее всего, построено на аналогии: база данных - база, склад, хранилище, что близко к действительности. Проводя простейшую аналогию, можно сказать, что база данных - это хранилище, где принимают взаимосвязанные данные, сортируют по темам и хранят в некотором порядке в одном месте, а также частично перерабатывают. Эти данные выдают строго по назначению и по требованию, оформленному согласно определенными правилами. Потребителю не обязательно знать в каком виде хранятся данные, при этом он решает какие данные, в каком количестве и в какой форме ему их нужно выдать. Это образное и, в общем, верное представление.

Основные идеи современных информационных технологий опираются на концепцию баз данных. Следовательно, базвом элементом информационных являются данные.

В основе концепции лежит механизм предоставления обрабатывающей программе из всех хранимых данных только тех, которые ей необходимы, и в форме, требуемой именно этой программе. Сама же формы описывается на логическом уровне, т.е. уровне, видимом из программы.

Одним из важнейших понятий в теории баз данных является понятие информации. 

*Информация* - это любые сведения о каком либо событии, процессе, объекте. Друми словами, это все, что может интересовать пользователя.

*Данные* - это информация, представленная в определенном виде. Для компьютерных технологий данные представлены в дискретном, фиксированном виде, удобном для хранения и обработки на компьютере, а также для передачи по каналам связи. 

Таким образом, база данных - это именованная совокупность данных, отражающая состояние объектов и их отношений в рассматриваемой предметной области.

Характерной чертой баз данных является постоянство:
- данные постоянно накапливаются и используются;
- состав и структура данных, необходимых для решения тех или иных прикладных задач, обычно постоянны во времени;
- отдельные или все элементы актуальности.

Т.е. речь идет о *признаке персистентности* данных в базе данных.

Таким образом, можно привести более точное определение базы данных, а именно, база данных - это совокупность взаимосвязанных устойчивых данных при наличии такой минимальной избыточности, которая допускает их независимое использование оптимальным образом для одного или нескольких приложений в определенной предметной области.
