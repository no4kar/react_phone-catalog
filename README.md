# Products catalog
## Description
Implementation Products catalog following [this design](https://www.figma.com/file/uEetgWenSRxk9jgiym6Yzp/Phone-catalog-redesign?node-id=1%3A2).

> Here is the [working DEMO](https://no4kar.github.io/react_phone-catalog/)

## Used for project
1. [React](https://legacy.reactjs.org/) main library that used for this project.
    - For simplicity, a functional approach is used throughout
1. [TS](https://legacy.reactjs.org/).
    - `JSDoc + // @ts-check` || `TS` || `without problems and safety` 
1. [React-router-dom](https://reactrouter.com/en/main).
    - to create a single-page application
    - interact with query and search params
1. [Redux](https://redux.js.org/) instead `React.createContext()`.
    - For simplicity data store management
    - The `Favorites` and `Cart` are used in many components, stored in localStorage, but managed in their own slices
1. [SASS](https://sass-lang.com/) external file is main approach for component's styling.
    - Only `./src/components/Slider/Slider.tsx` uses inline style object


    
  Redux - for state managment, loadsh, webpack
