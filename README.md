TypeScript React "material-ui" AutoComplete Demo
===================================

需要注意的是：

```
const [selected, setSelected] = useState<Option | null>(null)
```

此时必须显式传入`null`。如果写成`useState<Option|null>()`, 会报错：

```
Material-UI: A component is changing the uncontrolled value state of Autocomplete to be controlled.
```

由于通常我们习惯使用undefined来作为不存在的值，所以这里需要特别注意。

```
npm install
npm run demo
```
