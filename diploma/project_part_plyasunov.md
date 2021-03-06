 Каждая панель представлена в виде Page Frame отдельного XAML файла. Так как, панели состоят из трех компонентов(благодаря использованию MVVM паттерна), то стоит необходимость в разработке каждого файла для каждой компонента: View, Model и ViewModel.
 
 Model содержит описание модели данных для соответсвующего класса: определяется класс, внутри пространства имен проекта. Для Task, Employee и Departments были разработанны соответсвующие компоненты Model: TaskModel, EmployeeModel и Departments Model. Все свойства идентичны столбцам соответсвующих таблиц в базе данных. Не стоит забывать, что необходима реализаци интерфейса INotifyPropertyChange в каждом компоненте.
 
 Компонент View является представлением, которое содержит описание всех визуальных элементов панели: области ввода данных о задаче или сотруднике, информации об отделе и прочего. Он вставляется в главное окно путем привязки к истонику Frame. Данный компонент не связан напрямую с компонентом Model и не несет никакой функциональной и логической нагрузки. Представлен в XAML-файле как Page.
 
 Связующим View и Model компонентом является ViewModel. И именно в нем содержится весь функционал и логика, которая используются View. Компонент Model непосредственно поставляет данные компоненту ViewModel. Подключение ViewModel в View осуществляется через присваивание DataContext соответсвующего элемента класс ViewModel.
 
 Листинги каждого из компонентов вынесены в приложение.
 
 2.4.3 Контроллер RestClient и непосредственное обращение к серверу
 Чтобы не обременять компонент ViewModel функционалом, напрямую не относящимся не его задачам, нужно иметь в арсенале набор контроллеров, берущих на себя ответсвенность выполнения рутинных задач: установление соединения с серверов, отправки запросов и обработки ответов. Для этого был разработан контроллер RestClient, поддерживающий REST-API механизм взаимодействия с сервером.
 
 Так как в классе RestClient используются методы классов HttpWebResponse, HttpWebRequest, HttpClient и прочее, то в заголовке файла необходимо подключить библиотеки System.Net.Http. Для функции FormUrlEncodedContent, которая преобразуется данные для POST-запросов. 
 
 В самом контроллере описаны методы для POST и GET запросов, которые оптимизированны для использования компонентами ViewModel. Помимо методов имеются следующие поля:
 -  endPoint - конечная точка(IP адрес)
 -  httpVerb - перечисление методов запросов
 -  port - порт

2.4.4 Использование сторонних библиотек: NewtonJSON и MaterialDesign
Библиотека NewtonJSON является самой скачиваемой с платформы NuGet. Она крайне эффективно позволяет проводить сериализацию(упаковку) и десериализацию(распаковку) объектов.
Material Design - предоставляет огромное количество современных  элементов интерфейса и стилей для встраивания их в приложение.