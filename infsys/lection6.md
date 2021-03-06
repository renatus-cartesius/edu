# Ethernet: на витой паре и коаксиальном кабеле.
### Методы доступа в сетях
**Метод к передающей среде** - это метод, обеспечивающий выполнение совокупности правил, по которым узлы в сети получают доступ к ресурсу.

Существует два основных класса методов доступа:
1. Детерминированный
2. Недетерминированный(стохастический)

При детерминированных методах доступа передающая среда распределяется между узлами при помощи специального механизма управления, гаратирующего передачу данных узла в течении достаточно малого интервала времени.

Недетерминированные - это случайные методы доступа, предусматривающие конкуренцию всех узлов в сети за право передачи. Возможны одновременные попытки передачи со стороны нескольких узлов, в результате чего возникают коллизии. 
****
### Метод доступа CSMA/CD
Метод доступа, используемый в сетях Ethernet на разделяемой проводной среде называется CSMA/CD(множественный доступ с опознаванием несущей и обнаружением конфликтов - прослушивание несущей частоты с множественным доступом).

Механизм прослушивания среды и пауза между кадарам не гарантирует исключения ситуаций, когда две или более станций одновременно решают, что среда свободна и начинают передавать свои кадры. При этом происходит коллизия т.к. содержимое обоих кадров сталкивается на общем кабеле и происходит искажение информации.

### Ethernet 
Наибольшее распространение среди стандартных сетей получила сеть Ethernet. В первые она появилась в 1973 году как разработка комании Xerox. В 1985 году сеть Ethernet стала международным стандартом и получила называние IEEE802.3. Этот стандарт определяет множественный доступ к моноканалу типа "шина" с обнаружением конфликтов и контроля передачи. 
****
**Основные характеристики первоначального стандарта IEEE802.3.
**
- Топология: шина
- Среда передачи: коаксиальный кабель
- Скорость передачи: 10Мбит/сек. 
- Максимальная длина сети: 5 км
- Максимальное количество абонентов: до 1024.
- Длина сегмента сети: до 500 метров
- Количество абонетов в одном сегменте: до 100
- Метод доступа: CSMA/CD

****
В 1995 году появился дополнительный стандарт на более быструют версию Ethernet, работающий на скорости 100Мбит/в секунду (IEEE802.3u). 

В 1997 году появилась версия стандартов для скорости 1000Мбит/сек(IEEE802.3z)

****
Помимо стандартной топологии "шина" все шире применяются топологии типа "пассивная звезда" и "пассивное дерево". При этом предполагается использование репитеров и репиторных концентраторов, соединяющих между собой различные части сети. В результате может сформироваться древовидная структура сегментов разных типов. Максимальная длина кабеля сети может достигать до 3.5 км.

Доступ к сети Ethernet осуществляется по случайному методу CSMA/CD, обеспечивающему равноправие абонетов. В сети используются пакеты переменной длины