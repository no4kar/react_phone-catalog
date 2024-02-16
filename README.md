# Products catalog
## Description
Implementation Products catalog following [this design](https://www.figma.com/file/uEetgWenSRxk9jgiym6Yzp/Phone-catalog-redesign?node-id=1%3A2).

> Here is the [working DEMO](https://no4kar.github.io/react_phone-catalog/)

## Used for project
1. [React](https://legacy.reactjs.org/) main library that used for this project.
    - for simplicity, a functional approach is used throughout
1. [TS](https://legacy.reactjs.org/).
    -  `TS` || `JSDoc + // @ts-check` || `without problems and safety` 
1. [SASS](https://sass-lang.com/) external file is main approach for component's styling.
    - only `./src/components/Slider/Slider.tsx` uses inline style object
1. [React-router-dom](https://reactrouter.com/en/main).
    - to create a single-page application
    - interact with query and search params
1. [Redux](https://redux.js.org/) instead `React.createContext()`.
    - for simplicity data store management
    - the `Favorites` and `Cart` are used in many components, stored in localStorage, but managed in their own slices
    - interact with query and search params
1. [Lodash](https://lodash.com/) instead `React.createContext()`.
    - `lodash.debounce` for small search latency
    - `lodash.isequal` for [HOC](https://legacy.reactjs.org/docs/higher-order-components.html) [React.memo()](https://react.dev/reference/react/memo)
1. [Webpack](https://webpack.js.org/) for some tricks.
    - like this `const images = require.context(
  '../../images/banners', true,
  /\.(png|ico|svg|jpg|gif)$/,
);`
    - or like this `import varsScss from '../styles/utils/export.module.scss';`

## Additional
1. Products API implemented by standard httpClient but it easily can be overwriting with [axios](https://axios-http.com/docs/intro).
1. For DEMO only phones of one not very well-known brand are available on the server.
