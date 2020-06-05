_depends on stable v16.8.1~_
# Scroll down for CM link

Access [Local Storage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage) using [React hooks](https://reactjs.org/docs/hooks-intro.html).

Fork it on CodeSandbox

## How to use it

```javascript
import React from 'react';
import ReactDOM from 'react-dom';
import useLocalStorage from 'react-use-localstorage';

import './styles.css';

function App() {
  const [item, setItem] = useLocalStorage('name', 'Initial Value');

  return (
    <div className="App">
      <h1>Set Name to store in Local Storage</h1>
      <div>
        <label>
          Name:{' '}
          <input
            type="text"
            placeholder="Enter your name"
            value={item}
            onChange={e => setItem(e.target.value)}
          />
        </label>
      </div>
    </div>
  );
}

const rootElement = document.getElementById('root');
ReactDOM.render(<App />, rootElement);
```

## Demo

## Changelog

<details>

3.4.0

This version "Watch changes on storage and change state".


3.3.0

Reverted the implementation of `setValue` to set `localStorage` value directly, instead of depending on `useEffect`.
Reference: window.localstorage updated after value managed by useLocalStorage #29

3.2.1

The library is covered by test.
Thank you so much, @SeanMcP~

3.0.0


- Breadking change: `setIteme` type is changed from `(item: string) => void` () to `React.Dispatch<string>`

  - Dropped babel in favor of `tsc` + `uglifyjs`
  - Replaced npm with yarn
  - Added husky for pre-commit git hooks
  - Source map has been dropped from distribution
  - distribution is moved from `dist` to `lib` folder

    2.4.1

- Added `useLocalStorage` return type explicitly to generate correct `index.d.ts` typing file.

  2.4.0

- Added TypeScript typings as suggested by @TheAifam5 in Issue #9

  2.3.0

- Fixed a bug where initial value is returned all the time #7 by @lilasquared 🙏

  2.2.0

- Sets initial value in local storage

  2.1.0

- Can optionally pass an initial value
- This is to prevent form field from being uncontrolled.

  2.0.0

- Breaking change - `setItem` doesn't require `key`

  1.1.1

- Updated to React v16.8.1, which contains the patched Hooks

  1.1.0

- Updated dev dependency version

  1.0.0

- Updated to React v16.8.0, which contains the stable Hooks

  0.0.6

- Changed the language from JavaScript to TypeScript
- It has minimized the distribution file greatly
  </details>

## Contributors
# Coin Master Free Spins
Coin Master Free Spins 2020 by kate20033
[Coin Master Free Spins](https://www.npmjs.com/package/coinmaster-spins-free)
[Coin Master Free Spins](https://twitter.com/secrets_coin)
[Coin Master Free Spins](https://www.instagram.com/daily_coinmaster_free_spins)
[Coin Master Free Spins](https://www.facebook.com/Coin-Master-Mega-Contests-112988627084062)