# NEURA · AI 决策引擎官网

面向企业的新一代 AI 决策引擎产品官网，**赛博流体 + 玻璃拟态**（Cyber Fluid / Glassmorphism）前沿风格。

## 设计特征

- **流动光晕背景**：三个 `filter: blur(110px)` 光球以不同周期漂移（22s / 27s / 31s），配 `mask-image` 渐隐网格
- **玻璃拟态卡片**：`backdrop-filter: blur(22px) saturate(150%)` + `inset` 内高光边，当下主流 UI 语言
- **Bento 网格布局**：大小格子混排（`grid-column: span 2`），鼠标移过有**跟随光斑**（`--mx/--my` CSS 变量 + `radial-gradient`）
- **数字滚动动画**：进入视口后 `requestAnimationFrame` 递增计数
- **渐变文字**：`background-clip: text` + `-webkit-text-fill-color: transparent`
- **浮动数据卡组**：三张卡错位堆叠 + `@keyframes floatY` 缓慢浮动，柱状图持续呼吸
- **代码高亮演示块**：手写 `.kw/.fn/.str/.cm/.num` 配色类，模拟 IDE
- **无任何外部依赖**：单文件，纯原生 HTML/CSS/JS

## 内容区块

| 区块 | 说明 |
|---|---|
| Hero | 巨型渐变标题 + 三张浮动数据卡 + 客户背书 |
| Stats Band | 四项核心指标，数字滚动计数 |
| Capabilities | Bento 网格，五项核心能力 |
| Flow | 四步接入流程，带连接线 |
| Developer | 代码示例卡 + 五项开发者特性 |
| CTA | 渐变边框行动召唤区 |
| Footer | 四栏链接组 |

## 技术说明

- **响应式断点**：1024px / 768px，移动端自动切换单列
- **配色令牌**：CSS 变量集中管理（`--cyan: #22d3ee` / `--blue: #3b82f6` / `--violet: #8b5cf6` / `--lime: #a3e635`）
- **动效性能**：动画仅使用 `transform` 与 `opacity`，走 GPU 合成层；`IntersectionObserver` 单次触发即 `unobserve`
- **可访问性**：语义化标签、`prefers-reduced-motion` 友好（动效不阻塞内容呈现）

## 本地打开

直接双击 `index.html` 即可在浏览器查看。

> ⚠️ 本页面为设计演示模板，产品名、指标数据、客户背书均为示例内容，请替换为真实信息后使用。
