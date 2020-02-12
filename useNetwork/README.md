# @lchooks/use-network

React Hook to listen when the user goes online or offline.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-network`

#### npm

`npm i @lchooks/use-network`

## Usage

```js
import React from "react";
import useNetwork from "@lchooks/use-network";

function App() {
  const onNetworkChange = isOnline =>
    console.log(isOnline ? "Nomadcoders are back online" : "Nomadcoders just got offline");
  const isOnline = useNetwork(onNetworkChange);
  return <h1>{isOnline ? "Nomadcoders are online" : "Nomadcoders are offline"}</h1>;
}
```

### Arguments

| Argument        | Type     | Description                                           | Arguments          | Required |
| --------------- | -------- | ----------------------------------------------------- | ------------------ | -------- |
| onNetworkChange | function | Function to be called when the network status changes | isOnline : Boolean | no       |

### Return

| Return value | Type    | Description                                         | Default value |
| ------------ | ------- | --------------------------------------------------- | ------------- |
| isOnline     | Boolean | A boolean representing if the user is online or not | true          |