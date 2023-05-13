Описание
Класс Dropdown представляет выпадающий список, который может быть использован в веб-приложениях. Он реализует функциональность отображения и скрытия списка при клике на текущее значение списка, а также отображение выбранного элемента в текущем значении списка.

Конструктор
constructor(id: string)
Создает экземпляр класса Dropdown с указанным идентификатором.

Аргументы
id - строка, идентификатор элемента, в котором находится выпадающий список.
Свойства
this.dropdown - элемент выпадающего списка.
this.currentValue - элемент текущего значения списка.
this.currentValueText - элемент текста текущего значения списка.
this.list - элемент списка.
this.img - элемент изображения стрелки.
this.valueList - список элементов списка.
События
click - добавляет слушатель событий на элемент текущего значения списка и каждый элемент списка.
Методы
showList()
Показывает выпадающий список.

hideList()
Скрывает выпадающий список.

outsideClickListener(event: Event)
Слушатель событий для скрытия выпадающего списка при клике вне списка.

Аргументы
event - событие клика.
addClickListener()
Добавляет слушатель событий на документ для скрытия списка при клике вне списка.

removeClickListener()
Удаляет слушатель событий на документе для скрытия списка при клике вне списка.

Пример использования
javascript
Copy
import Dropdown from './dropdown.js';

const dropdown = new Dropdown('dropdown');
В этом примере мы импортируем класс Dropdown из модуля dropdown.js и создаем новый экземпляр класса с идентификатором элемента dropdown. Вызов конструктора инициализирует свойства объекта и добавляет слушатели событий на элементы списка.

HTML
html
Copy
<div id="dropdown">
  <div class="dropdown__current-value">
    <p>Option 1</p>
    <img src="arrow-down.svg">
  </div>
  <ul>
    <li class="selected">Option 1</li>
    <li>Option 2</li>
    <li>Option 3</li>
    <li>Option 4</li>
  </ul>
</div>
Это HTML-разметка выпадающего списка, которую использует класс Dropdown. Он содержит элемент текущего значения списка (<div class="dropdown__current-value">), который отображает текущее выбранное значение, и элемент списка (<ul>), содержащий элементы списка.

Как использовать
Создайте новый экземпляр класса Dropdown, передав идентификатор элемента списка в качестве аргумента конструктора.
Используйте HTML-разметку, указанную в примере, чтобы создать выпадающий список с элементами списка (<li>).
Добавьте стили для элементов списка.
Настраивайте функциональность списка, добавляя дополнительные методы и свойства в класс Dropdown.
Измените стили элементов списка и выпадающего списка, чтобы адаптировать его к вашим потребностям.
Заключение
Класс Dropdown представляет простой выпадающий список с функциональностью отображения и скрытия списка при клике на текущее значение списка, а также отображения выбранного элемента в текущем значении списка. Он может быть использован в веб-приложениях для выбора опций из предоставленного списка.