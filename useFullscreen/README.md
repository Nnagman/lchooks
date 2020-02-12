# @lchooks/use-fullscreen

React Hook to make any element go Fullscreen

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-fullscreen`

#### npm

`npm i @lchooks/use-fullscreen`

## Usage

```js
import React from "react";
import useFullscreen from "@lchooks/use-fullscreen";

function App() {
  const onChange = isFull =>
    console.log(isFull ? "Nomadcoders are in Fullscreen" : "Nomadcoders are not in Fullscreen");
  const { element, triggerFull, exitFull } = useFullscreen(onChange);
  return (
    <div ref={element}>
      <h1>Hello</h1>
      <button onClick={triggerFull}>Make this Fullscreen</button>
      <button onClick={exitFull}>Exit Fullscreen</button>
    </div>
  );
}
```

### Arguments

| Argument | Type     | Description                                                       | Arguments        | Required |
| -------- | -------- | ----------------------------------------------------------------- | ---------------- | -------- |
| onChange | function | Function to be called when the screen goes Fullscreen or exits is | isFull : Boolean | no       |

### Return

`useFullscreen` returns an object containing the following:

| Return value | Type      | Description                                                |
| ------------ | --------- | ---------------------------------------------------------- |
| element      | React Ref | Ref to add to the element that you want to make fullscreen |
| triggerFull  | Function  | Function to make the element enter fullscreen              |
| exitFull     | Function  | Function to make the document exit fullscreen              |