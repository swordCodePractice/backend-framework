---
id: deploy
title: 部署
url: https://www.yuque.com/mlgrgm/lrf0ra/ge1vor
---

部署功能是由sword cli操刀，sword cli是sword.js配套的伴生工具，如果你已经阅读了前面几个章节，就可以发现在开发模式下，初始化工程都是由cli完成的。sword.js的定位是一款跨多serverless平台（包括server）的nodejs框架，而且快速小巧一直是我们的主打，所以在部署方面我们用到了Esbuild，它可以帮助我们极快的transform我们的源代码，这个过程基本是瞬间完成，而且当我们使用cli初始化工程的时候，就已经有一个预先设置好的dockerfile在根目录，我们在server端只需要打包一个镜像就可以了～

<a name="suzte"></a>

## Server & Docker 🐳

```json
docker build -t sword/app .
```

<a name="HTfxG"></a>

## Server

```json
npm run build && npm run server
```
