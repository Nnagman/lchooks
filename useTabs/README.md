# @lchooks/use-tabs

React Hook to get currentItem when the user excuting a function.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-tabs`

#### npm

`npm i @lchooks/use-tabs`

## Usage

```js
import React from "react";
import useTabs from "@lchooks/use-tabs";

function App() {
  const { currentItem, changeItem } = useTabs(0, content);
  return (
    <div className="App">
      {content.map((section, index) => (
        <button onClick={() => changeItem(index)}>{section.tab}</button>
      ))}
      <div>{currentItem.content}</div>
    </div>
  );
}
```

### Arguments

| Argument  | Type     | Description                                         | Required |
| --------- | -------- | --------------------------------------------------- | -------- |
| initialTab   | string   | String which index should start with | no      |
| allTabs | map | map to show the user on the DOM      | yes      | 

### Return

| Return value | Type   | Description                                                             | Default value |
| ------------ | ------ | ----------------------------------------------------------------------- | ------------- |
| index, content | string | String to show the index of item and content of currentItem | `{currentItem:allTabs[currentIndex], changeItem:setCurrentIndex}`  |