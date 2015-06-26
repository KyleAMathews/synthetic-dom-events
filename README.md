# synthetic-dom-events

Forked from https://github.com/defunctzombie/synthetic-dom-events
so [can build in
Webpack.](https://github.com/defunctzombie/synthetic-dom-events/pull/10)

## example

```js
var event = require('synthetic-dom-events');

// event just returns a correctly created dom event object
// you are responsible for emitting it
var ev = event('click', { button: 2 });

var element = document.createElement('button');
element.dispatchEvent(ev);

// or legacy IE
//element.fireEvent('on' + ev.type, ev);
```
