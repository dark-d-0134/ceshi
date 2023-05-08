---
sidebar_position: 1
---

# markdown基础写法

## 代码块

### 代码块标题

```ts title="代码块标题"
function HelloCodeTitle(props) {
  // highlight-next-line
  return <h1>Hello, {props.name}</h1>;
}
```
### 代码块高亮
`// highlight-next-line`


### 代码块显示行号

`showLineNumbers=true`

```ts title="代码块显示行号" showLineNumbers=true
function HelloCodeTitle(props) {
  // highlight-next-line
  return <h1>Hello, {props.name}</h1>;
}
```

### 代码块隐藏复制按钮
`hideCopyButton=true`

```ts title="代码块隐藏复制按钮" hideCopyButton=true
function HelloCodeTitle(props) {
  // highlight-next-line
  return <h1>Hello, {props.name}</h1>;
}
```

### 实时编辑代码块
```markdown title="实时编辑代码块" showLineNumbers=true
<!-- 复制时去除tab位 -->
    ```jsx live
    function Clock(props) {
      const [date, setDate] = useState(new Date());
      useEffect(() => {
        const timerID = setInterval(() => tick(), 1000);

        return function cleanup() {
          clearInterval(timerID);
        };
      });

      function tick() {
        setDate(new Date());
      }

      return (
        <div>
          <h2>It is {date.toLocaleTimeString()}.</h2>
        </div>
      );
    }
    ```
```  
```jsx live
function Clock(props) {
  const [date, setDate] = useState(new Date());
  useEffect(() => {
    const timerID = setInterval(() => tick(), 1000);

    return function cleanup() {
      clearInterval(timerID);
    };
  });

  function tick() {
    setDate(new Date());
  }

  return (
    <div>
      <h2>It is {date.toLocaleTimeString()}.</h2>
    </div>
  );
}
```


## 选项卡

### 选项卡引入

```markdown title='Markdown Tabs'

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
  <TabItem value="apple" label="Apple" default>
    This is an apple 🍎
  </TabItem>
  <TabItem value="orange" label="Orange">
    This is an orange 🍊
  </TabItem>
  <TabItem value="banana" label="Banana">
    This is a banana 🍌
  </TabItem>
</Tabs>
    
```



## 告示

### 注意

```markdown  title='注意'

:::note

This is a note

:::
    
```

输出为

:::note

This is a note

:::

### 参照表
| color | type | value |
| ----- | ---- | ----- |
| 灰色  | note | 备注 |
| 绿色  | tip | 提示 |
| 蓝色  | info | 信息 |
| 黄色  | caution | 注意 |
| 红色  | danger | 危险 |


## 文本排版

### 标题

```markdown title='标题'
## 二级标题

### 三级标题

```
### 链接

```markdown title='链接'
[链接](https://www.baidu.com)
```

比如这个
[链接](https://www.baidu.com)

### 图片

```markdown title='图片'

![图片](https://www.baidu.com/img/bd_logo1.png)
```

比如这个
![图片](https://www.baidu.com/img/bd_logo1.png)

