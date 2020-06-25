# D3: Data-Driven Documents

<a href="https://d3js.org"><img src="https://d3js.org/logo.svg" align="left" hspace="10" vspace="6"></a>

**D3** (или **D3.js**) - это библиотека JavaScript для визуализации данных с использованием веб-стандартов. D3 поможет вам оживить данные, используя SVG, Canvas и HTML. 
D3 сочетает в себе мощные методы визуализации и взаимодействия с управляемым данными подходом к манипулированию DOM, предоставляя вам все возможности современных браузеров и свободу разработки правильного визуального интерфейса для ваших данных.

## Ресурсы

* [API Reference](https://github.com/d3/d3/blob/master/API.md)
* [Release Notes](https://github.com/d3/d3/releases)
* [Gallery](https://github.com/d3/d3/wiki/Gallery)
* [Examples](https://bl.ocks.org/mbostock)
* [Wiki](https://github.com/d3/d3/wiki)

## Установка

Если вы используете npm, `npm install d3`. В противном случае загрузите [последнюю версию](https://github.com/d3/d3/releases/latest).    
Выпущенный пакет поддерживает анонимные среды AMD, CommonJS и vanilla.    
Вы можете загрузить напрямую из [d3js.org](https://d3js.org), [CDNJS](https://cdnjs.com/libraries/d3), или [unpkg](https://unpkg.com/d3/). Например:

```html
<script src="https://d3js.org/d3.v5.js"></script>
```

Для минимизированной версии:

```html
<script src="https://d3js.org/d3.v5.min.js"></script>
```

Вы также можете использовать автономные микробиблиотеки D3. Например, [d3-selection](https://github.com/d3/d3-selection):

```html
<script src="https://d3js.org/d3-selection.v1.js"></script>
```

D3 написан с использованием [ES2015 модулей](http://www.2ality.com/2014/09/es6-modules-final.html).    
Создайте [пользовательский пакет, используя Rollup](https://bl.ocks.org/mbostock/bb09af4c39c79cffcde4), Webpack или предпочитаемый вами пакет.    
Чтобы импортировать D3 с помощью приложения ES-2015 введите специальные символы из конкретного модуля D3.

```js
import {scaleLinear} from "d3-scale";
```

Или импортировать все объекты в область имён (здесь, `d3`):

```js
import * as d3 from "d3";
```

В Node:

```js
var d3 = require("d3");
```

Вы также можете потребовать отдельные модули и объединить их в объект `d3`, используя [Object.assign](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign):

```js
var d3 = Object.assign({}, require("d3-format"), require("d3-geo"), require("d3-geo-projection"));
```
