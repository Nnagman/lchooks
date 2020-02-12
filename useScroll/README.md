# @lchooks/use-scroll

React Hook to get X/Y coordinates of current position of the scroll.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-scroll`

#### npm

`npm i @lchooks/use-scroll`

## Usage

```js
import React from "react";
import useScroll from "@lchooks/use-scroll";

function App() {
  const { x, y } = useScroll();
  return (
    <h1>
      nomadcoders are in: {x} / {y}
    </h1>
  );
}
```

### Return

| Return value | Type   | Description                                                             | Default value |
| ------------ | ------ | ----------------------------------------------------------------------- | ------------- |
| Coords       | Object | An object containing the x/y coordinates of the current scroll position | `{x:0, y:0}`  |