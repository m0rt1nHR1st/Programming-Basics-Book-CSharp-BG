#### Създаване на контролите за игра

Сега създаваме контролите за играта. Целта е да добавим **скролиращи ленти** (scroll bars), с които играчът се прицелва, и бутон за старт на **нова игра**. Затова трябва да редактираме файла **`Views/Home/Index.cshtml`**. Изтриваме всичко в него и въвеждаме кода от картинката:
  
![](/assets/chapter-7-images/15.Fruits-05.png) 

Този код създава уеб форма **`<form>`** със скролер (поле) **`position`** за задаване на число в интервала [**0 … 100**] и бутон [**Fire Top**] за изпращане на данните от формата към сървъра. Действието, което ще обработи данните, се казва **`Home/FireTop`**, което означава метод **`FireTop`** в контролер **`Home`**, който се намира във файла **`HomeController.cs`**. Следват още две подобни форми с бутони [**Fire Bottom**] и [**New Game**].
