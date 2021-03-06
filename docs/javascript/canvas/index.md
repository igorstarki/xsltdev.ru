---
description: В данном справочнике приводится информация о свойствах и методах объекта getContext(2d), который может использоваться для вывода в элементе canvas текста, линий, прямоугольников, кругов
---

# Свойства и методы Canvas 2D

HTML5 тег `<canvas>` используется для отображения графики на лету при помощи скриптов (обычно JavaScript).

Тем не менее, сам по себе элемент `<canvas>` не имеет инструментария для рисования. Это всего лишь контейнер для графики. Чтобы в действительности что-то нарисовать в элементе `<canvas>`, необходимо использовать соответствующий скрипт.

Метод `getContext()` возвращает объект, предоставляющий методы и свойства для рисования в элементе `<canvas>`.

В данном справочнике приводится информация о свойствах и методах объекта `getContext("2d")`, который может использоваться для вывода в элементе `<canvas>` текста, линий, прямоугольников, кругов и др.

Internet Explorer 9, Firefox, Opera, Chrome и Safari поддерживают элемент `<canvas>` и его свойства и методы. Internet Explorer 8 и более ранние версии не поддерживают элемент `<canvas>`.

## Цвета, стили, тени

Свойства:

[`fillStyle`](fillstyle.md)
: Устанавливает/возвращает цвет, градиент или шаблон, используемый для заливки графического объекта

[`shadowBlur`](shadowblur.md)
: Устанавливает/возвращает уровень размытости для теней

[`shadowColor`](shadowcolor.md)
: Устанавливает/возвращает цвет для теней

[`shadowOffsetX`](shadowoffsetx.md)
: Устанавливает/возвращает горизонтальное расстояние тени от фигуры

[`shadowOffsetY`](shadowoffsety.md)
: Устанавливает/возвращает вертикальное расстояние тени от фигуры

[`strokeStyle`](strokestyle.md)
: Устанавливает/возвращает цвет, градиент или шаблон, используемый для обводки фигуры

Методы:

[`addColorStop()`](<addcolorstop().md>)
: Определяет цвета и позицию остановки в объекте градиента

[`createLinearGradient()`](<createlineargradient().md>)
: Создает линейный градиент (для использования с содержимым элемента `<canvas>`)

[`createPattern()`](<createpattern().md>)
: Размножает заданный элемент в заданном направлении

[`createRadialGradient()`](<createradialgradient().md>)
: Создает радиальный/круговой градиент (для использования на содержимом элемента `<canvas>`)

## Стили линий

Свойства:

[`lineCap`](linecap.md)
: Устанавливает/возвращает стиль концов нарисованной линии

[`lineJoin`](linejoin.md)
: Устанавливает/возвращает тип угла, созданного пересечением двух линий

[`lineWidth`](linewidth.md)
: Устанавливает/возвращает ширину текущей линии

[`miterLimit`](miterlimit.md)
: Устанавливает/возвращает максимальную длину среза

## Прямоугольники

Методы:

[`clearRect()`](<clearrect().md>)
: Очищает заданную область пикселей внутри данного прямоугольника

[`fillRect()`](<fillrect().md>)
: Рисует "залитый" прямоугольник

[`rect()`](<rect().md>)
: Создает прямоугольник

[`strokeRect()`](<strokerect().md>)
: Рисует прямоугольник (без заливки)

## Контуры

Методы:

[`arc()`](<arc().md>)
: Создает дугу/кривую (используется для создания окружностей или их части)

[`arcTo()`](<arcto().md>)
: Создает дугу/кривую между двумя касательными

[`beginPath()`](<beginpath().md>)
: Начинает контур или сбрасывает текущий контур

[`bezierCurveTo()`](<beziercurveto().md>)
: Создает кубическую кривую Безье

[`clip()`](<clip().md>)
: Обрезает область любой формы и размера, находящуюся вне указанного контура

[`closePath()`](<closepath().md>)
: Замыкает контур соединяя последнюю точку с первой

[`fill()`](<fill().md>)
: Делает заливку текущей фигуры (контура)

[`isPointInPath()`](<ispointinpath().md>)
: Возвращает значение `true`, если заданная точка находится внутри текущего контура, в обратном случае возвращается значение `false`

[`lineTo()`](<lineto().md>)
: Добавляет новую точку контура и создает линию к этой точке от последней заданной точки

[`moveTo()`](<moveto().md>)
: Передвигает точку контура в заданные координаты не рисуя линию

[`quadraticCurveTo()`](<quadraticcurveto().md>)
: Создает квадратичную кривую Безье

[`stroke()`](<stroke().md>)
: В действительности рисует определенный вами контур

## Трансформации

Методы:

[`rotate()`](<rotate().md>)
: Поворачивает текущий графический объект

[`scale()`](<scale().md>)
: Изменяет масштаб текущего графического объекта

[`setTransform()`](<settransform().md>)
: Сбрасывает текущую матрицу трансформации в начальное состояние, а затем вызывает метод `transform()` с теми же параметрами

[`transform()`](<transform().md>)
: Применяет заданную матрицу трансформации

[`translate()`](<translate().md>)
: Ретранслирует позицию `(0,0)` в новое место

## Текст

Свойства:

[`font`](font.md)
: Устанавливает/возвращает свойства шрифта для текстового содержимого

[`textAlign`](textalign.md)
: Устанавливает/возвращает выравнивание для текстового содержимого

[`textBaseline`](textbaseline.md)
: Устанавливает/возвращает базовую линию, используемую при выводе текста

Методы:

[`fillText()`](<filltext().md>)
: Рисует текст с заливкой

[`measureText()`](<measuretext().md>)
: Возвращает объект, содержащий ширину заданного текста

[`strokeText()`](<stroketext().md>)
: Рисует текст без заливки

## Вывод изображений

Методы:

[`drawImage()`](<drawimage().md>)
: Рисует изображение, содержимое другого элемента `<canvas>` или видео

## Пиксельные манипуляции

Свойства:

[`data`](data.md)
: Возвращает объект, содержащий данные изображения заданного объекта `ImageData`

[`height`](height.md)
: Возвращает высоту объекта `ImageData`

[`width`](width.md)
: Возвращает ширину объекта `ImageData`

Методы:

[`createImageData()`](<createimagedata().md>)
: Создает новый, пустой объект `ImageData`

[`getImageData()`](<getimagedata().md>)
: Возвращает объект `ImageData`, который копирует пиксельные данные заданной прямоугольной области холста

[`putImageData()`](<putimagedata().md>)
: Помещает данные изображения (из заданного объекта `ImageData`) обратно в элемент `<canvas>`

## Компоновка

Свойства:

[`globalAlpha`](globalalpha.md)
: Устанавливает/возвращает текущее значение прозрачности или альфа-канала графического объекта

[`globalCompositeOperation`](globalcompositeoperation.md)
: Устанавливает/возвращает то, как исходное (новое) изображение нарисовано на целевом (существующем) изображении

## Другое

Методы:

[`save()`](<save().md>)
: Сохраняет состояние текущего контекста

[`restore()`](<restore().md>)
: Возвращает ранее сохраненное состояние и атрибуты

`createEvent()`

[`getContext()`](<getcontext().md>)
: Возвращает контекст рисования на холсте

[`toDataURL()`](<todataurl().md>)
: Возвращает URI данных, содержащий представление изображения в формате, заданном параметром типа
