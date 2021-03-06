# Протокол STP
Протокол связующего (остовного) дерева (Spanning Tree Protocol. STP).
- Автоматическое отключение дублирующие соединений в Ethernet
- Связующее дерево - подграф без циклов содеражищий все вершины исходного графа.
Преимущества
- Надежность соединений между коммутаторами
- Защита от ошибок конфигурации

Состояния портов в STP
**Listening** - порт обрабатывающий BPDU, но не передает данные
**Learning** - порт не передает кадры, но изучает MAC-адреса в поступающих кадрах и формирует таблицу коммутации
**Forwarding** - порт принимает и передает кадры данных и BPDU.
**Blocking** - порт заблокирован чтобы избежать кольцевого соединения
**Disabled** - порт выключен администратором

WIFI как интерфейс в OSI расположен в подуровне управления логическим каналом и подуровнем управления доступом к среде.

WIFI
- доминирующая технология беспроводной переедачи данных в локальных сетях
- IEEE 802.11

Физический уровень WIFI
 - 6 разных стандартов IEEE 802.11
 
 Канальный уровень WIFI
 - Метод CSMA/CA
 - Протокол MACA
 - Формат кадра WIFI
 - Сервисы WIFI

### Особенности беспроводной среды
Вероятность ошибки передачи выше, чем в проводной среде.
Мощность предаваемого сигнала намного выше, чем принимаемого
Ограниченный диапазон распространения сигнала - не все компьютеры в сети получают данные
- Проблема скрытой станции
- Проблема засвеченной станции