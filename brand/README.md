# CairnPack 品牌指南

> 本文是团队 CairnPack 的品牌规则：名称写法、品牌价值、slogan、写作守则与标识。各产品（Gebinde、Haytham Core、Haytham Launcher）的名称规则、定位与产品文案写在各自的 repo，和本文冲突时以本文为准。
>
> 决定日期：2026-10-16 起草，2026-10-18 从 Haytham Launcher 的品牌指南拆出，成为团队共用的版本。

## 名称

团队名称一律写 **CairnPack**：正文、README、版权声明（`CairnPack contributors`）、NuGet 包 ID 与 `<Authors>` 都是这个写法。只有本来就不分大小写、惯例用小写的地方保持小写：域名 `cairnpack.dev`、URL，以及跟着域名反写的标识符（`dev.cairnpack.*`）。

| 用途 | 写法 |
|---|---|
| 团队 | **CairnPack** |
| GitHub org | `CairnPack` |
| 主域名 | `cairnpack.dev` |
| NuGet 包 ID 前缀 | `CairnPack.`（例如 `CairnPack.Gebinde`） |
| 版权人 | `CairnPack contributors` |

理由：

- GitHub org 注册时就是 `CairnPack`，org 页面、clone URL 与 repo 页面都显示这个大小写；正文跟着它写，不必改 org 名称。
- 字标 `cairn PACK` 本来就分成两段。
- repo 名（`HaythamCore`、`HaythamLauncher`）与 .NET 前缀也用 PascalCase，英文句首也不必为了全小写的名称改写句子。
- GitHub org 用团队名称而不用产品名：所有产品都放在同一个 org，日后增减产品也不必改。

### 考虑过但不采用

- **团队名称只用 Cairn**：最有力的理由是短，和叠石的意象、slogan 最贴。不采用：Cairn 是旧产品的名字，团队也叫 Cairn，会让人以为 Cairn 是产品、Haytham 是它改名后的版本；cairn 又是普通英文单词，账号、域名都已被占，Steam 上还有一款叫 *Cairn* 的游戏，很难搜到。
- **全小写 cairnpack**：最有力的理由是和域名完全相同，只有一种写法。不采用：GitHub org 已经注册成 `CairnPack`；团队名称不会出现在命令或文件名里，域名本来就不分大小写，搜 cairnpack 一样找得到。
- **NuGet 前缀写成 `Cairnpack.`**：把团队名称当成一个词、只大写开头，是专有名词的一般写法。不采用：它和 org、正文的写法都不同，等于第三种写法。

## 身份

核心维护者主导、社区共建：方向与质量由维护者把关，社区可以贡献代码。第一人称用“我们”。

- 不选“独立开发者、第一人称‘我’”：和社区开放矛盾。
- 不选“社区治理”：精雕细琢需要有人守住质量标准。

## 品牌价值

总纲是**开发者友好**，底下有三个价值。它们是做决定时的判断标准，对外则靠具体做法表现，不另外写成品牌故事。

| 价值 | 意思 | 对外的具体做法 |
|---|---|---|
| **聆听** | 每个需求都会得到**回应**，但不保证每个都会实现 | 每个 issue 都会得到三种答复之一：会做、不做（附上理由）、之后再说。不在对外文案里写回复期限 |
| **精雕细琢** | 每一处交互都仔细打磨 | 让人亲眼看到，而不是自己说出来；界面改动附上前后截图或录像 |
| **社区开放** | 欢迎每一位开发者一起打磨 | 代码以 GPL-3.0-or-later 开源并接受贡献 |

可以用三连句做宣传：

> *Every request, heard. Every detail, polished. Every developer, welcome.*

每一句都要有上表的做法撑腰（写进 CONTRIBUTING.md 与 issue 模板），否则就只是口号。

### 考虑过但不采用

- **可复现、透明、不绑定当品牌价值**：它们都有实际功能可以佐证。不采用：这些是功能，竞品迟早做得出来；态度比较难被复制。它们改当产品各自的承诺。
- **用名字讲品牌故事**（“cairn 是石堆路标，每个人放一颗石头……”）：可以让名字自己说出价值。不采用：太有营销味，开源工具很少这样说话。

## Slogan

- **英文**：**Many Stones. One Foundation.**
- **中文**：**叠石为记，与你同行。**（以中文另外撰写，不是翻译；四四节奏）

Slogan 来自 cairn（叠石路标）的意象，属于团队，不属于某个产品；产品用各自的一句话介绍与产品承诺。

## 写作守则

适用于团队与所有产品对外的文字：README、网站、界面文案、错误信息、发布说明。

- **具体**：每句都点名一个用户认得的东西（clone、git diff、tag、Modrinth）和一个看得到的结果；不用 reproducible、seamless、powerful 这类抽象词。
- **语气温和而精确**：内容像工程文档一样严谨，口吻像有经验、不卖弄的前辈；可以轻巧，但不玩梗，不用 emoji。
- **错误信息**：说清楚发生了什么、为什么、下一步怎么做；永远不怪用户。语气不随浅色／深色主题改变。
- **语言**：英文是母版。中文另外撰写：简中为母版，繁中做本地化（连用词都换，例如“服务器”→“伺服器”、“文件”→“檔案”、“设置”→“設定”），不只是转换字形。
- **名称**：不取中文名，中文文案直接用英文名称；不标注发音；不写名称由来。名称不含 Minecraft、mine，也避开 craft（Mojang 的使用规范不允许产品名称含 Minecraft；craft 在这个生态里太拥挤）。

## 视觉

- **Minecraft 味只取“形”**：等角方块、体素可以用；不用像素字、草地或泥土材质、苦力怕等游戏元素；不模仿 Minecraft 的 logo。
- **颜色**：品牌色只有薄荷绿 `#b0eebf`；浅色背景上的字标用深绿 `#133f23`，深色背景上用薄荷绿。产品界面的配色由各产品的设计系统决定。

## 标识

2026-10-18 定稿。文件都在本目录：

| 文件 | 用途 |
|---|---|
| `banner/cairnpack-banner-pack-light.png`／`-dark.png` | 「cairn PACK」banner，浅色／深色主题（org 首页用这组） |
| `banner/cairnpack-banner-clear-light.png`／`-dark.png` | 「cairn」banner，浅色／深色主题 |
| `banner/*.svg` | 上面各张图的矢量原稿 |
| `wordmark/cairn-pack-wordmark*.svg` | 「cairn PACK」字标：深绿、`-mint`、`-black`、`-white` |
| `wordmark/cairn-wordmark*.svg` | 「cairn」字标：深绿、`-mint`、`-black`、`-white` |
| `wordmark/*.png` | 深绿与薄荷两色的透明底 PNG，约为 SVG 的 2 倍 |

SVG 都是纯路径，不含文字、字体或外部图片，可以直接嵌入。素材的授权与商标政策尚未决定。

### 字标

写成 `cairn` 和 `cairn PACK`：「cairn」用小写字母，但放大到大写高度，和后面的大写「PACK」一样高（做法参考 nVIDIA、7-ELEVEn）。只有 i 的点超出顶线。

- **c**：正圆，开口 54°。字距从笔画端点量起，所以 c 可以贴近 a。
- **a**：单层 a，碗是窄椭圆（宽 = 高 × 0.86）。碗两侧竖笔是 0.9 倍粗，上下横笔是 0.92 倍粗。
- **i**：直笔顶到大写高度，点在顶线上方。
- **r**：肩部半径 0.34（以大写高度为单位），和 n 的肩部一样圆。
- **n**：宽 0.68。
- **PACK**：P 的碗为 0.62 见方；A 是窄 A；C 是 0.9 宽的椭圆，开口 36°，比 c 收得更紧，看起来不空；K 的两笔是 60°。
- 字距（单位是 x-height，即大写高度 ÷ 1.4）：

  | 字距 | ca | ai | ir | rn | 词距 | PA | AC | CK |
  |---|---|---|---|---|---|---|---|---|
  | 值 | 0.04 | 0.2 | 0.26 | 0.12 | 0.46 | −0.08 | −0.02 | 0.02 |

### Banner

slime 图标加上字标，透明底。字标的大写高度是 slime C 高度的 0.6，上下居中对齐 C。

- PNG 是 2560×800（画布 1280×400 的 2 倍）。
- 「cairn」banner 的 slime 每格 16 px，「cairn PACK」每格 14 px，都落在整数像素上。

### org 首页

[`profile/README.md`](../profile/README.md) 顶部的 banner 用 `<picture>` 按访客的浅色或深色主题切换：

```html
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./cairnpack-banner-pack-dark.png">
    <img alt="cairnpack" src="./cairnpack-banner-pack-light.png" width="720">
  </picture>
</p>
```

`profile/` 里的两张 PNG 是 `banner/` 同名文件的副本：改了 banner，要把副本一起换掉。要改用「cairn」banner，把副本换成 `clear` 那组，并把 `pack` 换成 `clear`。
