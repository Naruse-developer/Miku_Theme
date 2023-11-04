# Miku_theme

The frontend of ServerStatus-Hotaru based on Vue 3.0

基于Vue 3.0和Semantic UI打造的”船新“ServerStatus主题，基於原模板进行修改。

本仓库存放了ServerStatus-Hotaru默认主题的源码。

关于本仓库默认使用的图片素材的说明请见下方项目仓库。

关于自定义主题：

如果仅修改标题、副标题、页脚和更新数据的间隔，可以直接修改根目录下的`config.js`文件。其他如更换素材、背景图片、对其他文字的修改等建议修改本仓库代码并重新打包

原模板：

https://github.com/cokemine/hotaru_theme

### 功能 (Function)
样式更新

ver 2.0

新增模板 : マジカルミライ 2023 图片来源 : https://magicalmirai.com/2023/
> [!WARNING]  
> 图片包含版权 , 请勿用于商用 ! ! !

安全修补程式

ver 1.21 发布于2023-11-4

Commit : https://github.com/Naruse-developer/Miku_Theme/commit/7f97a963dc0b797a457b9a0bd9263ef2bde574ce

Ver 1.2 发布于2022-9-30

Regular Expression Denial of Service (CVE-2022-25858)

Commit : https://github.com/Naruse-developer/Miku_theme/commit/259ca053a8da54b1ebe6971562f17f01bc50b26c

Ver 1.1 发布于2022-06-24

Ver 1.0 发布于2022-06-23

这里添加了额外的小功能

1. 当前默认语言为中文（繁体），简体中文和英语会在之后发布
2. 当服务器的负载达到0.4以上和1.4以上时会有警告色 （黄色和橘红色），方便了解更多信息.

### 功能自定义 (Customization)

想要更换警告色的触发条件或者颜色 , 请修改下列文件即可

```javascript
*/src/components/TableItem.vue
```

### 安装 (Install)

使用这个探针主题前需要安装可乐大佬的探针脚本
请前往 ServerStatus-Hotaru: https://github.com/CokeMine/ServerStatus-Hotaru

### 替换前端样式 (Replace style)

请前往Releases页面下载最新的样式 (已经包含代码提示)

https://github.com/Naruse-developer/Miku_Theme/releases/

### 碎碎念 (Other)

服务端在某些CPU处理效能较差的情况下可能会有数据不更新,服务端停止的情况

**请使用防火墙只允许客户端的IP进入即可.**

### 效果演示 (Preview)

新版本样式

![](https://github.com/Naruse-developer/Warframe_theme/blob/master/demo/demo.png)
图片来源 : https://magicalmirai.com/2023/

> [!WARNING]  
> 图片包含版权 , 请勿用于商用 ! ! !

旧版本样式

![](https://github.com/Naruse-developer/Warframe_theme/blob/master/demo/old.png)

原图来源 (Source)
https://mobile.twitter.com/moitoi/status/1375518164516175874/photo/1

## Project setup
```
npm install or npm i
```

*If you think the installation is taking longer than expected, download **node_modules.zip** Skip this step*

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
