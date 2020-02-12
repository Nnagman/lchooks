# @lchooks/use-input

React Hook to get value which user entered and check validate.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-input`

#### npm

`npm i @lchooks/use-input`

## Usage

```js
import React from "react";
import useInput from "@lchooks/use-input";

function App() {
  const maxLen = value => value.length <= 20;
  const name = useInput("Nomadcoders", maxLen);
  return (
    <div className="App">
      <h1>Hi</h1>
      <input placeholder="hey" {...name} />
    </div>
  );
}
```

### Arguments

| Argument  | Type     | Description                                         | Required |
| --------- | -------- | --------------------------------------------------- | -------- |
| initialValue   | string   | Default string | yes      |
| validator | function | Function to check validate value which entered by user | no  | 

### Return

| Return value | Type   | Description                                                             | Default value |
| ------------ | ------ | ----------------------------------------------------------------------- | ------------- |
| value | string | String which entered by user | null  |
| onChange | function | Fucntion to get value which entered by user | null  |