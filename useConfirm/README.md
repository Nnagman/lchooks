# @lchooks/use-confirm

React Hook to ask the user for a confirmation before executing a function.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-confirm`

#### npm

`npm i @lchooks/use-confirm`

## Usage

```js
import React from "react";
import useConfirm from "@lchooks/use-confirm";

function App() {
  const deleteWorld = () => console.log("Deleting world...");
  const confirmDelete = useConfirm("Are you sure?", deleteWorld);
  return <button onClick={confirmDelete}>Delete the world</button>;
}
```

### Arguments

| Argument  | Type     | Description                                         | Required |
| --------- | -------- | --------------------------------------------------- | -------- |
| message   | string   | Message to show the user on the confirmation propmt | yes      |
| onConfirm | function | Function to be executed when the user confirms      | yes      |
| onCancel  | function | Function to be executed when the user cancels       | no       |

### Return

| Return value | Type     | Description                                    | Default value |
| ------------ | -------- | ---------------------------------------------- | ------------- |
| function     | function | Function wrapped around the confirmation logic | null          |