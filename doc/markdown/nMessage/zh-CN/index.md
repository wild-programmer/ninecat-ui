
# Message 信息提示

用于页面信息提示。

## 何时使用

页面中需要有操作提示或者信息提示的时候使用。

## 代码演示

:::demo
```html
<template>
  <n-button @click="openMessage">Open Message</n-button>
</template>
<script>
  export default {
    methods: {
      openMessage(){
        this.$nMessage({
          type: 'info',
          message: '打开了提示框...',
        })
      }
    }
  }
</script>
```
:::

## API

| 参数 | 说明 | 类型 | 默认值 |
| :--- | :--- | :--- | :--- |
| type | 信息类型,可选值`info`,`success`,`warning`,`error` | String | info |
| message| 信息内容 | String |  |
| duration| 信息展示的时间（ms） | Number | 3000 |