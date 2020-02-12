# @lchooks/use-before-leave

React Hook to execute a function when the mouse leaves the page. Useful to show a popup or for analytics.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-before-leave`

#### npm

`npm i @lchooks/use-before-leave`

## Usage

```js
import React from "react";
import useBeforeLeave from "@lchooks/use-before-leave";

function App() {
  const beforeLeave = () => console.log("User is leaving...");
  useBeforeLeave(beforeLeave);
  return <h1>Hello lchooks</h1>;
}
```

### Arguments

| Argument      | Type     | Description                                              | Required |
| ------------- | -------- | -------------------------------------------------------- | -------- |
| onBeforeLeave | function | Function to be called when the mouse leaves the document | yes      |