# Warframe_theme

The frontend of ServerStatus-Hotaru based on Vue 3.0

基于Vue 3.0和Semantic UI打造的”船新“ServerStatus主题，模仿了可乐大佬主题样式。

本仓库存放了ServerStatus-Hotaru默认主题的源码。

关于本仓库默认使用的图片素材的说明请见下方项目仓库。

关于自定义主题：

如果仅修改标题、副标题、页脚和更新数据的间隔，可以直接修改根目录下的`config.js`文件。其他如更换素材、背景图片、对其他文字的修改等建议修改本仓库代码并重新打包。

ServerStatus-Hotaru: https://github.com/CokeMine/ServerStatus-Hotaru

原模板：

https://github.com/cokemine/hotaru_theme

### 功能 (Function)

这里添加了额外的小功能

Ver 1.0 发布于2022-06-23

1. 当前默认语言为中文（繁体），简体中文和英语会在之后发布
2. 当服务器的负载达到0.4以上和1.4以上时会有警告色 （黄色和橘红色），方便了解更多信息.

### 功能自定义 (customization)
想要更换警告色的条件或者颜色 ， 请修改下列文件

```bash
*/src/components/TableItem.vue
```

## 效果演示

![](https://github.com/Naruse-developer/Warframe_theme/blob/master/demo/demo.png)

原图来源 (Source)
https://mobile.twitter.com/moitoi/status/1375518164516175874/photo/1

## Project setup
```
npm install or npm install --force
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```