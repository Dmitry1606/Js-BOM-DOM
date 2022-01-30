 // Задание 1
// Просмотрите в консоли браузера объект navigator. Найдите информацию о своем браузере, системе.
// Просмотрите в консоли браузера объект location. Найдите в этом объекте текущий url, где вы находитесь.
// Выведите в консоль строку:
// С помощью браузера ... я открыл страничку ... 
// (необходимые значения добавьте с помощью BOM)

console.log(`С помощью браузера ${navigator.userAgent} я открыл страничку ${location.href}`);



// Задание 2
// В файле html есть разметка:
// <ul id="list">
// <li>Джон</li>
// <li>Пит</li>
// <li>Джессика</li>
// <li>Сара</li>
// </ul>
// Вывести в консоль каждое из имен (содержимое каждого li).

// // Задание 3
// // Поменять имена в списке выше на числа от 0 по порядку (0, 1, 2 и т.д.)

let listItems = document.querySelectorAll('li')

for (let li of listItems) {
    console.log(li);
    // }


    for (let i = 0; i < listItems.length; i++) {
        listItems[i].innerText = i
    }



    // // Задание 4
    // // Написать функцию, которая принимает на вход 3 параметра: название тега, название цвета, содержимое. Функция должна сформировать необходимый тег, добавить необходимый стиль с цветом и внести содержимое. Вывести несколько таких сгенерированных тегов в консоль, затем отправить их на страницу.


    function createArray(tag, color, text) {
        let newTag = document.createElement(tag);
        document.newTag.style.background = color;
        newTag.innerText = text;
        return newTag;
        // document.body.appendChild(newTag)
    }
    let p = createArray('p', 'red', 'something')
    document.body.appendChild(p);


    // Задание 5
    // Создать с помощью js абзац (тег p). Добавить в него контент. Добавить к нему стили: размер 36px, жирный шрифт. Добавить абзац с текстом на страницу.

    let newTAG = document.createElement('p');
    document.newTAG.style.fontWeight = 'bold'
    document.newTAG.style.fontSize = '36px'
    newTAG.innerText = 'hdgfhdfhfhfjhjfhfhffhfhfh';
    return newTAG
    let P = filterFor('p', 'bold', '36px')
    document.body.appendChild(newTAG);


    // Задание 6
    // Вставить в страницу (в html документ) тег <select>. С помощью js добавить в этот select опции (option) под годы от 1960 по 2020.

    let select = document.querySelector('select');
    for (let i = 1960; i < 2021; i++) {
        let option = documentCreateElement('option');
        option.innerText = i
        select.appendChild(option)
    }

    // Задание 7
    // Вставить в страницу (в html документ) ul.
    // Предусмотреть в коде следующий массив:
    // Перебирать массив, для каждой ячейки массива создать li, наполнить li текстом:
    // - Клиент Женя оплатил заказ
    // - Клиент Павел отменил заказ
    // ... остальные li с контентом
    // Маска получается такой: "Клиент ИМЯ СТАТУС заказ", где имя - свойство объекта (а объект здесь - это текущая ячейка массива), статус зависит от от свойства order: если true – то оплатил, если false – то отменил.
    let shoppers = [{
        name: "Женя",
        order: true
    },
    {
        name: "Кристина",
        order: true
    },
    {
        name: "Павел",
        order: false
    },
    {
        name: "Виолетта",
        order: false
    },
    {
        name: "Костя",
        order: true
    }];

    let ul = document.querySelector('ul')
    let paid;
    for (let i = 0; i < shoppers.length; i++) {
        if (shoppers[i].order) {
            paid = 'оплатил '
        } else { paid = 'отменил' }
        let li = document.createElement('li');
        li.innerText = `клиент ${shoppers[i].name} ${paid} заказ`
        ul.appendChild(li)
    }


    // Задание 8
    // Есть массив ссылок:
    // Вам нужно:
    // 1) при помощи JS создать DIV, задать ему css стили (фон, паддинги)
    // 2) при помощи цикла пройтись по массиву 'linksArr', для каждого из элементов массива сформировать ссылку (тег
    // c атрибутом href и текстом из массива) и добавить эту ссылку в созданный DIV из пункта 1
    // При нажатии на ссылки адреса должны открываться в новой вкладке (атрибут target="_blank")
    // ПОДСКАЗКА Для создания атрибута используется js метод setAttribute:
    // element.setAttribute(name, value) - где name - сам атрибут, который нужно добавить, value - его значение.
    // Вкладывать ссылки в див нужно с помощью метода appendChild или append.
    // 3) Добавить DIV из пункта 1 (со ссылками внутри ) в BODY

    let linksArr = ['https://www.onliner.by/', 'https://www.youtube.com/', 'https://vk.com/', 'https://www.google.com/', 'https://yandex.ru/'];


    let div = document.createElement('div');
    div.style.padding = '30px';
    div.style.background = 'pink';

    for (let i = 0; i < linksArr.length; i++) {
        let a = document.createElement('a');
        a.setAttribute('href', linksArr[i]);
        a.innerText = linksArr[i];
        div.appendChild(a)
    }
    document.body.appendChild(div)



    // Задание 9
    // Добавить к нескольким тегам на странице класс "forRemove". Далее написать JS код, который найдет в HTML все элементы с классом "forRemove" и удалит их.
    // ПОДСКАЗКА Для удаления DOM-элементов можно использовать метод element.remove()


    let elemnts = document.querySelectorAll('.forRemove')
    for (let i = 0; i < elements.length; i++)
        elements[i].remove();





    // Задание 10*
    // Создать массив объектов с полями name, age. Создать html таблицу с двумя колонками,
    // заполненную этими объектами. Name должно быть красного цвета, age - синего.

    let users = [{ name: 'Andrei', age: 23 }, { name: 'Petya', age: 27 }]

    let table = document.createElement('table');
    for (let i = 0; i < users.length; i++) {
        let tr = document.createElement('tr');
        let td = document.createElement('td');
        let tdName = document.createElement('td');
        let tdAge = document.createElement('td');
        tdName.innerText = users[i].name;
        tdAge.innerText = users[i].age;
        tr.append(tdName);
        tr.append(tdAge);
        tdName.style.color = 'red';
        tdAge.style.color = 'blue';
        table.append(tr);
    }
    document.body.append(table);
