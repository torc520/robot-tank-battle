# 机器人坦克大战（网页版）

**直接玩：<https://torc520.github.io/robot-tank-battle/>**

Godot 4 导出的网页版坦克大战。白色机器人是你，黑色是敌人，守住底部基地、打光一波波敌人。
手机横屏玩：屏幕任意位置滑动=走一格，轻点=开火，右下角有大圆开火键；电脑上 WASD + 空格，也支持手柄。

## 文件说明

| 文件 | 说明 |
| --- | --- |
| `index.html` | 入口，站点根就是本仓库根目录 |
| `index.js` / `index.wasm` | Godot 引擎（wasm 37.7 MB，Pages 会 gzip 到约 10 MB） |
| `index.pck` | 游戏本体资源 |
| `manifest.json` | 横屏 + 全屏声明（安卓上点“点我打横”按钮可强制横屏） |
| `index.audio.*.worklet.js` | 音频线程脚本 |
| `index.icon.png` / `index.apple-touch-icon.png` / `index.png` | 图标与加载图 |

## 部署方式

GitHub Pages，Deploy from a branch，分支 `main`，目录 `/ (root)`。
文件是用 Git Data API 传的（网页上传单文件上限 25 MB，37.7 MB 的 wasm 会被拒）。