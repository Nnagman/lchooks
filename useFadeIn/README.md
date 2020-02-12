# @lchooks/use-fade-in

React Hook to fade in any element.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-fade-in`

#### npm

`npm i @lchooks/use-fade-in`

## Usage

```js
import React from "react";
import useFadeIn from "@lchooks/use-fade-in";

function App() {
  const fadeIn = useFadeIn(5, 10);
  return <h1 {...fadeIn}>This will fade in.</h1>;
}
```

### Arguments

| Argument | Type   | Description                                     | Required | Default value |
| -------- | ------ | ----------------------------------------------- | -------- | ------------- |
| duration | number | Sets the duration of the transition. In seconds | no       | 1             |
| delay    | number | Delays of transition's start. In seconds        | no       | 0             |

### Return

`useScroll` returns an object containing the following:

| Name  | Type      | Description                                                               |
| ----- | --------- | ------------------------------------------------------------------------- |
| ref   | React Ref | A ref created to fadeIn the element                                       |
| style | Object    | Style object containing `{opacity:0}` to give to the element as a default |

It's recommended to just spread the returned object on the element as shown in the Usage section above.