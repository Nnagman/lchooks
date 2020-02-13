# @lchooks/use-axios

React Hook to request data asynchronous And Refetch when the user executing a function.

노마드코더 수업을 들으면서 클론코딩했습니다.
Thank you nomadcoders!!
https://academy.nomadcoders.co/p/introduction-to-react-hooks

## Installation

#### yarn

`yarn add @lchooks/use-axios`

#### npm

`npm i @lchooks/use-axios`

## Usage

```js
import React from "react";
import useAxios from "@lchooks/use-axios";

function App() {
  const { loading, data, error, refetch } = useAxios({
    url: "https://yts.mx/api/v2/list_movies.json"
  });
  return (
    <div className="App">
      <h1>{data && data.status}</h1>
      <h2>{loading && "Loading"}</h2>
      <button onClick={refetch}>Refetch</button>
    </div>
  );
}
```

### Arguments

| Argument  | Type     | Description                                         | Required | Default value |
| --------- | -------- | --------------------------------------------------- | -------- | ------------- |
| opt   | array   | Array to request using Axios | yes      | null |
| axiosInstacne | axios | Axios for Asynchronous Processing | no      | defaultAxios |

### Return

| Return value | Type   | Description                                                             | Default value |
| ------------ | ------ | ----------------------------------------------------------------------- | ------------- |
| state | Object | An object containing the response value | null
| refetch | Function | An function to refetch | null  |