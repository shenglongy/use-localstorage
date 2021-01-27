# use-localstorage

A Hook for persisting state into localStorage.

## Install

``` sh
$ npm install --save @shenglong/use-localstorage
```

Or with Yarn

``` sh
$ yarn add @shenglong/use-localstorage
```

## Usage

```javascript
import useLocalStorage from "@shenglong/use-localstorage"

function App() {
  const [name, setName] = useLocalStorage('name', 'Bob');

  return (
    <input
      type="text"
      placeholder="Enter your name"
      value={name}
      onChange={e => setName(e.target.value)}
    />
  )
}
```
