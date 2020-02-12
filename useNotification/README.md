# @lchooks/use-notification

React Hook to request data asynchronous And Refetch when the user executing a function.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-notification`

#### npm

`npm i @lchooks/use-notification`

## Usage

```js
import React from "react";
import useNotification from "@lchooks/use-notification";

function App() {
  const triggerNotif = useNotification("Thank you Nomadcoders", {
    body: "notification~"
  });
  return (
    <div className="App">
      <button onClick={triggerNotif}>notification</button>
    </div>
  );
}
```

### Arguments

| Argument  | Type     | Description                                         | Required |
| --------- | -------- | --------------------------------------------------- | -------- |
| title   | string   | String to show the user on the notification prompt | yes      |
| options | array | array to be executed optional      | no      |

### Return

| Return value | Type   | Description                                                             | Default value |
| ------------ | ------ | ----------------------------------------------------------------------- | ------------- |
| Notification       | Object | An object containing the notification title and options | null  |