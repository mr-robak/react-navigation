# `@react-navigation/devtools`

Developer tools for React Navigation.

## Installation

Open a Terminal in your project's folder and run,

```sh
yarn add @react-navigation/devtools
```

## Usage

For redux dev tools extension integration, you can pass a ref to the container:

```js
import * as React from 'react';
import { NavigationContainer } from '@react-navigation/native';
import { useReduxDevtoolsExtension } from '@react-navigation/native';

export default function App() {
  const navigationRef = React.useRef();

  useReduxDevtoolsExtension(navigationRef);

  return (
    <NavigationContainer ref={navigationRef}>{/* ... */}</NavigationContainer>
  );
}
```
