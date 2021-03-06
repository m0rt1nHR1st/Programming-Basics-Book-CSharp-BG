#### Генериране на случайни плодове

Трябва да генерираме случайни плодове. За да направим това, трябва да напишем метод **`GenerateRandomFruits()`** с кода от картинката по-долу. Този код записва в таблицата (матрицата) **`fruits`** имена на различни картинки и така изгражда игралното поле. Във всяка клетка от таблицата се записва една от следните стойности: **`apple`, `banana`, `orange`, `kiwi`, `empty` или `dynamite`**. След това, за да се нарисува съответното изображение в изгледа, към текста от таблицата ще се долепи **`.png`** и така ще се получи името на файла с картинката, която да се вмъкне в HTML страницата като част от игралното поле. Попълването на игралното поле (9 колони с по 3 реда) става в изгледа **`Index.cshtml`** с два вложени **`for`** цикъла (за ред и за колона).

За да се генерират случайни плодове за всяка клетка се генерира **случайно число** между 0 и 8 (вж. класа **`Random`** в .NET). Ако числото e 0 или 1, се слага **`аpple`**, ако е между 2 и 3, се слага **`banana`** и т.н. Ако числото е 8, се поставя **`dynamite`**. Така плодовете се появяват 2 пъти по-често отколкото динамита. Ето и кода:

![](/assets/chapter-7-images/15.Fruits-07.png) 