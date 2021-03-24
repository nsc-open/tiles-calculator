通过指定范围，可以计算指定源地图在一定 level 范围内的所有切片地址，可用于地图离线使用。
提供多个语言的版本，在不同平台使用。

分两个部分：
1. 切片计算（切片数量、预估总文件体积）
2. 切片下载（主要包含了一些反爬的技巧）

参考 API：

```js
const result = calculateTiles({
  source: '', // 天地图 xx底图
  extent: [],
  minLevel: 1,
  maxLevel: 1,
  returnFullPath: true // 是否返回全的切片地址，如果为否的话，只返回 xyz 信息
})
```