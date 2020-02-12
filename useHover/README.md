# @lchooks/use-hover

React Hook to detect a hover on an any React Element

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-hover`

#### npm

`npm i @lchooks/use-hover`

## Usage

```js
import React from "react";
import useHover from "@lchooks/use-hover";

function App() {
  const onHover = () => console.log("Nomadcoders hovered!");
  const markedRef = useClick(onHover);
  return <h1 ref={markedRef}>Hello Nomadcoders</h1>;
}
```

### Arguments

| Argument | Type     | Description                                       | Required |
| -------- | -------- | ------------------------------------------------- | -------- |
| onHover  | function | Function to be called when the element is hovered | yes      |

### Return

| Return value | Type      | Description                                                     | Default value |
| ------------ | --------- | --------------------------------------------------------------- | ------------- |
| ref          | React Ref | A React Ref listening to the hover event, add it to any element | null          |