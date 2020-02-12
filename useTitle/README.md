# @lchooks/use-title

React Hook to update your document's title.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-title`

#### npm

`npm i @lchooks/use-title`

## Usage

```js
import React from "react";
import useTitle from "@lchooks/use-title";

function App() {
  useTitle("Thank you nomadcoders!!");
  return <h1>Welcome</h1>;
}
```

### Arguments

| Argument | Type   | Description                                | Required |
| -------- | ------ | ------------------------------------------ | -------- |
| title    | string | The title you want to use on your document | yes      |