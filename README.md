# RA2WEB CUSTOM AI

本仓库基于Supalosa的AI方案深度改造实现，不求基于AI自定义的解析，直接基于ts编写定制化的攻防逻辑

## 开发状态

目前已经支持海军

## 安装说明

请使用Node.js 20版本，推荐使用nvm管理Node版本，方便切换。

建议使用官方原版红色警戒2安装，作为本地调试AI的资源。如果你更改了游戏ini，那么可能无法运行，请知悉！

```sh
npm install
npm run build
npx cross-env MIX_DIR="C:\指向你安装的红色警戒2目录" npm start
```

这将创建一个回放（`.rpl`）文件，可以[导入到实际游戏中](https://game.chronodivide.com/)。

## 与机器人对战

如果你真正有兴趣与机器人对战（无论是这个机器人还是你自己的机器人），请联系 Chrono Divide 的开发者以获取详细信息。

## 调试

```sh
npx cross-env MIX_DIR="C:\指向你安装的红色警戒2目录" npm --node-options="${NODE_OPTIONS} --inspect" start
```

## 发布

将 npmjs token 放在 ~/.npmrc 或适当的位置。

```bash
npm publish
```
