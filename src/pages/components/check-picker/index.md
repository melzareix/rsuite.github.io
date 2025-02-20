# CheckPicker 多项选择器

用于多项数据选择，支持分组。

- `<CheckPicker>`

## 获取组件

```js
import { CheckPicker } from 'rsuite';
```

## 演示

<!--{demo}-->

## Props

### `<CheckPicker>`

| 属性名称             | 类型`(默认值)`                                                        | 描述                                 |
| -------------------- | --------------------------------------------------------------------- | ------------------------------------ |
| appearance           | enum: 'default', 'subtle' `('default')`                               | 设置外观                             |
| block                | boolean                                                               | 堵塞整行                             |
| classPrefix          | string `('picker')`                                                   | 组件 CSS 类的前缀                    |
| cleanable            | boolean `(true)`                                                      | 可以清除                             |
| container            | HTMLElement or (() => HTMLElement)                                    | 设置渲染的容器                       |
| data \*              | Array&lt;[DataItemType](#types)&gt;                                   | 组件数据                             |
| defaultValue         | string[]                                                              | 设置默认值 `非受控`                  |
| disabled             | boolean                                                               | 禁用组件                             |
| disabledItemValues   | string[]                                                              | 禁用选项                             |
| groupBy              | string                                                                | 设置分组条件在 `data` 中的 `key`     |
| labelKey             | string `('label')`                                                    | 设置选项显示内容在 `data` 中的 `key` |
| menuClassName        | string                                                                | 应用于菜单 DOM 节点的 css class      |
| menuStyle            | Object                                                                | 应用于菜单 DOM 节点的 style          |
| maxHeight            | number `(320)`                                                        | 设置 Dropdown 的最大高度             |
| onChange             | (value:string, event)=>void                                           | `value` 发生改变时的回调函数         |
| onClose              | ()=>void                                                              | 关闭回调函数                         |
| onClean              | (event:SyntheticEvent)=>void                                          | 值清理时触发回调                     |
| onGroupTitleClick    | (event)=>void                                                         | 点击分组标题的回调函数               |
| onOpen               | ()=>void                                                              | 打开回调函数                         |
| onSearch             | (searchKeyword:string, event)=>void                                   | 搜索的回调函数                       |
| onSelect             | (value:string, item: [DataItemType](#types) , event)=>void            | 选项被点击选择后的回调函数           |
| placeholder          | React.Node `('Select')`                                               | 占位符                               |
| placement            | enum: [Placement](#types)`('bottomStart')`                            | 位置                                 |
| preventOverflow      | boolean                                                               | 防止浮动元素溢出                     |
| renderExtraFooter    | ()=>React.Node                                                        | 自定义页脚内容                       |
| renderMenu           | (menu:React.Node)=>React.Node                                         | 自定义渲染菜单列表                   |
| renderMenuGroup      | (groupTitle:React.Node, item:[DataItemType](#types))=>React.Node      | 自定义选项组                         |
| renderMenuItem       | (label:React.Node, item: [DataItemType](#types))=>React.Node          | 自定义选项                           |
| renderValue          | (value: any[], items: any[],selectedElement:React.Node) => React.Node | 自定义被选中的选项                   |
| searchable           | boolean `(true)`                                                      | 可以搜索                             |
| sticky               | boolean                                                               | 把选项中已选择的选项置顶在最前面     |
| sort                 | (isGroup: boolean) => (a: any, b: any) => number                      | 对选项排序                           |
| size                 | enum: 'lg', 'md', 'sm', 'xs' `('md')`                                 | 设置组件尺寸                         |
| toggleComponentClass | React.ElementType `('a')`                                             | 为组件自定义元素类型                 |
| value                | string[]                                                              | 设置值 `受控`                        |
| valueKey             | string `('value')`                                                    | 设置选项值在 `data` 中的 `key`       |
