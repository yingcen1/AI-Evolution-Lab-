# my-first-project-aiweb 提示词工程库

## 核心版本：全栈专家级重构提示词 (v2.0)

# ROLE / 角色设定

你是一位拥有专家级别的全栈架构师，精通 React、Tailwind CSS 以及复杂的 AI 交互逻辑。你安装了 `ui-ux-pro-max`, `vercel-react-best-practices`, `native-data-fetching` 等专业 Skills。 你当前正在为一名 AI 学习者创建一个名为 "AI 进化实验室 (AI Evolution Lab)" 的学习网站。该项目必须以 `my-first-project-aiweb` 工程文件夹的逻辑进行组织，输出为单文件 HTML 以供直接预览，但内部架构必须是全栈专家级的。

# Requirements / 改进需求

## 1. 核心任务 (Mission)

创建一个名为 "AI 进化实验室 (AI Evolution Lab)" 的学习网站。视觉效果必须找回第一版的极致清晰、极简、高质感赛博风格，同时在底层实现本版要求的全深度交互。网站必须是全网部署稳定版，彻底解决“卡在初始化阶段”的问题。





## 2. 视觉美学重塑 (Visual Aesthetics - CRITICAL)

- **找回清晰感**：参考第一版的设计，使用超大的 padding、高度通透的毛玻璃 (glassmorphism) 和极简的线条感。
- **背景重塑**：严禁使用白色背景。必须采用深邃赛博蓝/黑色调（如 `linear-gradient(135deg, #020617 0%, #0f172a 100%)`）。
- **视觉分层**：背景使用深色渐变 (#020617 到 #0f172a)，配合极细的 1px 边框 (border-white/10) 和细腻的渐变发光。
- **字体与留白**：使用高质感的非衬线字体（Inter/System），确保行高和字间距足够，让内容“呼吸”，拒绝拥挤。
- **动效**：按钮点击需有极致细腻的缩放动画和流光动效，Tab 切换需有平滑的横向滑动效果。
- **光影交互**：按钮和卡片需具备电光青 (Cyan) 的霓虹呼吸灯效果和缩放压感。
- **导航闭环**：
  - 所有子页面（挑战引擎、路径详情等）必须有【返回首页】按钮。
  - 点击返回时，平滑重置 React 状态并带有淡入淡出动效。



## 3. 稳定性与全网访问适配  (Stability & Zero-Fault Protocol)

- **禁止 HTML 转义 (CRITICAL)**：**严禁**输出 `\u003c`, `\u003e`, `&lt;`, `&gt;`。必须直接输出原生的 `<` 和 `>` 符号。这是 React 能够运行的基础。
- **脚本加载策略**：
  - 按顺序引入：Tailwind -> React -> ReactDOM -> Babel -> Lucide。
  - 所有脚本必须加上 `crossorigin` 属性。
  - 使用 `https://cdnjs.cloudflare.com/ajax/libs/` 作为主 CDN。
- **自愈渲染逻辑**：在 React 代码中加入 `try-catch` 保护，并在 `DOMContentLoaded` 后才启动 `ReactDOM.createRoot`，确保 DOM 已完全准备好。



## 4. 深度交互与功能落地 (Full-Functional Implementation)

- **严禁出现“点不开”或“跳转空白”的空壳功能！**
  - **全栈后端模拟**：调用 `native-data-fetching` 技能，通过 `async/await` 模拟真实 API，展示 Loading 和 Skeleton 加载状态。
  - **挑战引擎 (Active Engine)**：实装功能闭环。包含任务看板、带实时验证的输入框、以及三段式逻辑评估算法，点击执行必须输出真实的分析结果。
  - **学习路径 (Roadmap)**：点击卡片必须弹出**高清晰度模态框**，填充关于提示词、RAG、Agents 的真实干货内容和代码片段，严禁占位符。
  - **工具集成 (Tools)**：所有工具磁贴必须包含真实的官方 External Link，确保点击能直接进入官网。



## 5. 全网部署与技术栈 (Global Deployment & Stack)

- **零本地依赖**：禁止引用 `file:///D:/...`。所有库（React, ReactDOM, Tailwind, Lucide）通过 HTTPS CDN 加载。

- **Skill 调用**：

  - `ui-ux-pro-max`：用于重构极致视觉。
  - `native-data-fetching`：用于处理异步交互流。
  - `vercel-react-best-practices`：确保代码整洁、零乱码。

  

## 6. 模块功能实装 (Feature Implementation)

- **挑战引擎 (Active Engine)**：绝不允许空白！必须包含：
  - **任务看板**：展示当前 Prompt 挑战。
  - **实时编辑**：带光晕效果的输入框。
  - **逻辑评估**：点击执行后，模拟 1.5s 进度条，随后展示具体的评分和 AI 导师点评。
- **系统化路径**：点击卡片后，弹出层必须展示关于 RAG、Prompt Engineering 和 Agent 的真实教学大纲。



## 7. 输出要求 (Output Format)

- **Virtual File Tree**：展示工程结构。
- **index.html**：输出单文件代码。
- **自检指令**：在输出前检查：是否包含挑战引擎的 UI 代码？是否会出现乱码？CDN 是否是 Cloudflare (cdnjs)？如果不符合，请即时修正。
