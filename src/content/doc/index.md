---
title: ReactDoc 文档网站
---

基于react.dev官方项目，适用于开发文档、组件库页面的模版项目

## 编写md文档 {/*编写md文档*/}
- 在 `src/content` 目录下面新建文件夹,使用 markdown 编写文档
- markdown 文件内部支持使用 react 组件，组件需要在 `src/components/MDX/MDXComponents` 下注册

## 侧边栏 {/*侧边栏*/}
- 在 `src/sidebarConfig` 中配置你的侧边栏菜单数据, 并在 `pages/[[...markdownPath]].js` 下面引入侧边菜单数据
## 主页 {/*主页*/}
- 在 `src/components/Layout/HomeContent.js` 配置你的主页内容

## 顶部导航栏 {/*顶部导航栏*/}
- 在 `src/components/Layout/TopNav/TopNav.tsx` 配置你的顶部导航栏内容

## sandpack代码沙箱 {/*使用sandpack在线代码沙箱*/}
- 通过`src/components/MDX/Sandpack/SandpackRoot`添加你的组件库依赖, 在线预览你的组件库组件

<Sandpack>

```js
import { Button } from 'ysol';

export default function App() {
    return <Button>点击</Button>
}
```

</Sandpack>