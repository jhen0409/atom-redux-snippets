# Atom Redux Snippets

Atom snippets for [Redux](https://github.com/gaearon/redux). This snippets uses Babel(ES2015, ES2016), CoffeeScript, LiveScript syntax.

## Support Language

 - Babel (ES2015, ES2016)
 - CoffeeScript
 - LiveScript

## Usage

 - import redux (rdx-ipt)
```js
import { ${1:applyMiddleware, createStore, combineReducers, compose, bindActionCreators} } from 'redux';
```
 - import react-redux (rdx-iptc)
```js
import { ${1:Provider, connect} } from 'react-redux';
```

 - action (rdx-act)
```js
export function ${1:addTodo}($2) {
  $4

  return {
    $3
  };
}
```
 - async-action (rdx-acta)
```js
export function ${1:addTodo}($2) {
  return (dispatch, getState) => {
    $4

    dispatch({
      $3
    });
  };
}
```
 - action-type (rdx-tp)
```js
export const $1 = '$1';$2
```
 - actions-map (rdx-map)
```js
const actionsMap = {
  [$1]: (state, action) => {
    $2
  }
};
```
 - map-action (rdx-mapact)
```js
[$1]: (state, action) => {
  $2
}
```
 - reducer (rdxer)
```js
export default function ${1:todos}(state = initialState, action) {
  $2

  return state;
}
```
 - middleware (rdx-mdw)
```js
export default function $1({ dispatch, getState }) {
  return next => action => {

    ${2: next(action);}
  };
}
```

about LiveScript, CoffeeScript snippets generated code, see [live.cson](snippets/live.cson) and [coffee.cson](snippets/coffee.cson).

## LICENSE

[MIT](LICENSE)