# To do приложение
___
## hw1: HTML
- Реализована вертка страницы по [дизайну](https://github.com/ok-technopolis-autumn-2022/todo-app-design) figma 
- Настроено accessibility
___
## hw2: CSS
- Реализована стилизация приложения в соответствии с макетом
___
## hw3: Препроцессоры CSS
- Был установлен менеджер пакетов `npm` и выполнена инициализация `npm init`
- Установлен препроцессор `sass`
- Установлен сборщик модулей `parsel`
- Выполнен переход к `style.scss`
- В `style.scss` проведена оптимизация повторяющихся частей, а также добавлены переменные. К формату `scss` аналогично приведены файлы нормализации и шрифтов. 
___
## hw4+hw5: JS
Реализована архитектура на основе паттерна `Observer`.
Имеем три составных части - модели, хранилище и компоненты.

- `index.js` - точка входа. Создаем App, где внутри создаются экземпляры компонентов. 
- В `components` содержатся все операции с изменением задач. Когда обновляется состояние, запускается render.
- `models` это наши задачи с параметрами и статусы.   
- `Store` содержит состояние задач и `Observer`. 
- Класс `Observer` хранит подписчиков и наблюдает за изменением состояния в store. 
- Как только меняется состояние, Observer будет запускать каждый subscriber и обновлять представление. 
