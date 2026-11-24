# DEAD PRECINCT · 亡城警署

![cover](screenshots/cover.jpg)

一款 **PS1 风格的复古生存恐怖网页游戏 Demo**，致敬 1998 年的经典生存恐怖游戏。
整个游戏是**一个约 570 KB 的 HTML 文件**：零依赖、零外部资源，下载后双击即可在浏览器里游玩（电脑、手机均可）。

> 本项目是一次**人智协同（Human × AI）开发实验**：由一个人与 Anthropic 的 Claude **Fable 5.2** 和 **Opus 5.5** 两个模型接力，在一天内迭代六个版本完成。

| | | |
|---|---|---|
| ![](screenshots/street.jpg) | ![](screenshots/zombie-grab.jpg) | ![](screenshots/alarm-corridor.jpg) |
| ![](screenshots/garage-boss.jpg) | ![](screenshots/characters.jpg) | ![](screenshots/portrait.jpg) |

## 怎么玩

- **在线**：开启本仓库的 GitHub Pages 后，访问 `https://<用户名>.github.io/<仓库名>/`
- **本地**：下载 `index.html`，用 Chrome / Edge / Safari 打开
- 声音需在第一次点击或按键后才会开始（浏览器规定）；iPhone 请关闭静音键

| 操作 | 键盘 | 手机 |
|---|---|---|
| 前进 / 后退 | ↑ ↓ | 方向盘 上 / 下 |
| 原地转身 | ← → | 方向盘 左 / 右 |
| 跑 | Shift | □（开关） |
| 举枪（自动瞄准） | 按住 空格 | R1（开关） |
| 调查 / 开门 / 射击 | J 或 回车 | ✕ |
| 背包 | I | ○ |

流程约 10 分钟：中央大街 → 警署大厅（安全屋）→ 西侧办公室 → 东走廊 → 武器库 → 地下车库 Boss 战。

## 特点

- **PS1 画面还原**：320×240 渲染、顶点抖动、15 位色抖动、仿射贴图扭曲、CRT 扫描线与颗粒
- **坦克式操作 + 固定机位 + 第一人称开门过场**
- **Blender 预渲染背景**：10 个固定机位背景由 Blender Cycles 离线渲染后调色，实时 3D 角色叠加并按深度遮挡
- **分段低多边形角色**：女警、两种丧尸、原创怪物“爬行者”“镇暴者”，贴图全部由代码逐像素绘制
- **全部声音实时合成**：三首原创配乐（探索 / 安全屋 / Boss）、混响、共振峰人声（呻吟、惨叫、咆哮）、环境音、心跳
- **恐怖演出**：装死丧尸起身、破窗突袭、警报红灯、全场断电后 Boss 现身；被咬时以抓咬动作和音效表现

## 开发过程（人智协同）

| 版本 | 内容 | 模型 |
|---|---|---|
| v1–v2 | 自研 WebGL 渲染器、玩法与流程、光照与材质 | Fable 5.2 |
| v3–v4 | 固定机位、Blender 预渲染背景（人在本机渲染）与调色合成 | Fable 5.2 / Opus 5.5 |
| v5–v6 | 角色贴图与分段建模、音频重做、恐怖演出 | Opus 5.5 |

人负责定方向、做审美判断、在本机跑渲染和体验；AI 负责设计、实现与自测。

## 已知不足

手感偏僵硬、建模仍较粗糙、配乐不够丰富；未在所有手机机型上完整测试。欢迎提 Issue 或 PR。

## 声明

本作为非商业的同人致敬作品，所有角色、怪物、地名与音乐均为原创，与任何游戏公司无关联，未使用任何原作素材。

## License

[MIT](LICENSE)

---

# DEAD PRECINCT (English)

A **PS1-style retro survival-horror browser game demo** — the entire game is a **single ~570 KB HTML file** with no dependencies. Download `index.html` and double-click to play (desktop or mobile).

Built in one day as a **human × AI collaboration** between one human and Anthropic's Claude **Fable 5.2** and **Opus 5.5**, across six iterations.

**Features:** 320×240 rendering with vertex jitter, 15-bit dithering, affine texture warping and CRT scanlines · tank controls, fixed cameras and first-person door transitions · Blender (Cycles) pre-rendered backgrounds with depth-correct real-time characters · segmented low-poly characters with code-painted textures · fully synthesized audio (original score, formant voices, ambience) · original monsters and characters only.

**Controls:** arrows to move/turn, Shift to run, hold Space to aim (auto-target), J/Enter to act/shoot, I for inventory; on-screen pad on mobile.

Non-commercial fan tribute; all characters, monsters, places and music are original. Licensed under MIT.
