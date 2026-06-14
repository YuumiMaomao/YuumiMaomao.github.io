# 个人作品集网站 — 结构蓝图

> **设计方向**：Renaissance × 现代 UI（古典油画气质 + 极简高级感）
> **技术参考**：`renaissance-ui` skill 规范
> **配色**：奶白 #F5F0E8 · 墨黑 #1A1612 · 金色 #C9A84C · 褐棕 #8B6F4E
> **字体**：Bebas Neue（展示大标题）· Playfair Display Italic（强调）· Space Mono（标签/标注）

---

## 全局结构

```
导航（固定浮动胶囊）
  ↓
P1–2   Hero 封面
  ↓
P3     内容营销 — 微信板块
  ↓
P3     内容营销 — 抖音板块
  ↓
P4     内容营销 — 小红书板块 + 作品墙
  ↓
P5     AI 工作流（短链）
  ↓
P6     AI 工作流（长链）
  ↓
P7–8   更多技能 + 其他经历
  ↓
P9     未来能做的事
  ↓
P10    联系页（欢迎来找我玩）
```

---

## 导航

**样式**：浮动胶囊，不贴顶，`mt-6 mx-auto rounded-full`，背景 `rgba(245,240,232,0.85)` + `backdrop-blur`

**链接锚点**：
| 标签 | 锚点 |
|------|------|
| 内容营销 | `#content-marketing` |
| AI 工作流 | `#ai-workflow` |
| 技能 & 经历 | `#skills` |
| 未来规划 | `#future` |
| 联系我 | `#contact` |

---

## P1–2 · Hero 封面（全屏）

**占比**：约 2 屏高，视觉冲击入口

**图片**：`image1.png`（主视觉大图，全出血背景）

**文案排版**：
```
[超大 Bebas Neue]
很高兴认识你

[Playfair Display Italic · 副标题]
陈有米 Yuumi · 品牌内容营销 × AI 工作流

[Space Mono · 小标签]
BRAND CONTENT  ·  AI WORKFLOW  ·  MARKETING
```

**交互**：
- 滚动入场：translate-y + blur + opacity 三联动画
- 向下滚动指示箭头（细线风格）

---

## P3 · 精通3平台品牌内容营销

**section id**：`content-marketing`

### 板块标题
```
[Bebas Neue · 大]  精通3平台品牌内容营销
[Space Mono · 小标签]  WECHAT · DOUYIN · XIAOHONGSHU
```

---

### 微信（1、微信）

**布局**：4列卡片横排，每张卡片 = 封面图 + 链接按钮

**文案**：`点开看详情～`

**卡片内容**（4张，均为竖版封面图）：

| 卡片 | 图片 | 链接 |
|------|------|------|
| 微信卡片 1 | `image2.jpeg` | https://mp.weixin.qq.com/s/nhW3Yp0ckwHWro4tE6qUNg |
| 微信卡片 2 | `image3.jpeg` | https://mp.weixin.qq.com/s/xBoLoW_NHIt1F4dutp5fwQ |
| 微信卡片 3 | `image4.jpeg` | https://mp.weixin.qq.com/s/199hBVE7zpXsEP8_nsLLYg |
| 微信卡片 4 | `image5.jpeg` | https://mp.weixin.qq.com/s/ync3qg83CePAOwD4QCxDVA |

**卡片交互**：
- 悬停：整体 `scale(0.98)` + 金色边框出现
- 点击：新标签页打开链接
- Double-Bezel 卡片样式（外壳奶白 + 内核图片）

---

### 抖音（2、抖音）

**布局**：横版大图全宽展示（`image6.jpeg`）

**文案**：标签 `DOUYIN`

**备注**：横版截图展示抖音主页/数据面板，不带跳转链接

---

## P4 · 小红书 + 作品墙

### 小红书（3、小红书）

**布局**：4列卡片横排，同微信卡片样式

**文案**：`点开看详情～`

**卡片内容**（4张，竖版封面图）：

| 卡片 | 图片 | 链接 |
|------|------|------|
| 小红书卡片 1 | `image7.png` | http://xhslink.com/o/5zeqq9PsaRY |
| 小红书卡片 2 | `image8.png` | http://xhslink.com/o/6x0MK37o7pF |
| 小红书卡片 3 | `image9.png` | http://xhslink.com/o/5hZnQCWHrJm |
| 小红书卡片 4 | `image10.png` | http://xhslink.com/o/50HfShAN2d3 |

---

### 作品墙

**布局**：全宽大图 `image11.jpeg`，展示更多作品拼图

**样式**：图片上方留 `Space Mono` 标签 `PORTFOLIO WALL`

---

## P5 · AI 工作流（短链）

**section id**：`ai-workflow`

**流程说明**：
```
参考图 → 语言模型提取风格提示词 → 文生图 → 产品校准 → 图生视频 → 剪映后期
```

**流程图图片**（横排，5格）：

| 步骤 | 图片 | 说明 |
|------|------|------|
| Step 1 参考图 | `image12.png` | 原始参考素材 |
| Step 2 提示词 | `image13.png` | 语言模型提取风格 |
| Step 3 文生图 | `image14.png` | AI 生成图像 |
| Step 4 产品校准 | `image15.png` | 校准产品细节 |
| Step 5 成品预览 | *(视频文件：啊啊啊啊啊.mov，不可嵌入)* | 点击查看成品 |

**成品展示**：
- 图片：`image16.png`（小红书封面竖图）
- 链接：http://xhslink.com/o/41lxGTrPkEL
- 文案：`点击查看成品`

**其他AI图文作品**（3列卡片）：

| 卡片 | 图片 | 链接 |
|------|------|------|
| AI图文 1 | `image17.png` | http://xhslink.com/o/1XsbzJzQfm3 |
| AI图文 2 | `image18.png` | http://xhslink.com/o/3zyhraDh6x4 |
| AI图文 3 | `image19.png` | http://xhslink.com/o/6BkUFc2Nhde |

---

## P6 · AI 工作流（长链）

**流程说明**：
```
原始创意 → 分镜脚本 → AI线稿 → AI分镜图 → AI图生视频 → 剪映后期及配乐
```

**流程图图片**（横排，6格）：

| 步骤 | 图片 | 说明 |
|------|------|------|
| Step 1 原始创意 | `image20.jpeg` | 手绘或参考素材 |
| Step 2 分镜脚本 | `image21.png` | 文字分镜稿 |
| Step 3 AI线稿 | `image22.png` | AI生成线稿 |
| Step 4 AI分镜图 | `image23.png` | AI精绘分镜 |
| Step 5–6 成片 | *(视频文件，不可嵌入)* | 点击查看成品 |

**成品展示**：
- 图片：`image24.png`（小红书竖版封面）
- 链接：http://xhslink.com/o/3AClNDDK6sH
- 文案：`点击查看成品`

**其他AI视频作品**（3列卡片）：

| 卡片 | 图片 | 链接 |
|------|------|------|
| AI视频 1 | `image25.png` | http://xhslink.com/o/4deR6NjghyO |
| AI视频 2 | `image26.png` | http://xhslink.com/o/6AwFgmVvFfV |
| AI视频 3 | `image27.png` | http://xhslink.com/o/26ANeUwwp4z |

---

## P7–8 · 更多技能 + 其他经历

**section id**：`skills`

### 更多品牌技能（2×2 网格）

| 技能 | 图片 | 描述 |
|------|------|------|
| 🎯 品牌策划 | `image28.png` | 市场调研、策略优化、方案落地 |
| 📱 媒介运营 | `image29.png` | 抖音直播、小红书投放、数据分析 |
| 🚀 跨界合作 | `image30.png` | 品牌联名、快闪活动、周边开发 |
| 🛠️ 项目管理 | `image31.png` | SOP梳理、流程优化、知识库 |

**样式**：Double-Bezel 大卡片，图片作为卡片背景，文字叠加

### 其他经历（3列横排）

| 品牌 | 图片 |
|------|------|
| 奶糖派 | `image32.png` |
| 银河集团 | `image33.png` |
| 行动派 | `image34.png` |

**样式**：logo 卡片，奶白背景，细线边框，悬停金色描边

---

## P9 · 未来能做的事

**section id**：`future`

**大标题**：
```
[Bebas Neue]  未来能做的事
[Playfair Italic]  AI赋能，从内容生产到营销玩法
```

**三项内容**（竖向堆叠，编号 + 标题 + 详情）：

**1. 搭建内容AI数据中心，高品质一站式发布流**
> 依据品牌规范，制定标准化生文、生图、生脚本、生视频要求，批量审阅及发布

**2. 多模态调用Skill和MCP连接内外部数据API，辅助经营提效**
> CRM、DP等自动分析内部最新经营数值，同行竞品数据快速深度调研，发现市场机会点

**3. 汇报及营销场景vibe/spec coding，推动项目决策和落地**
> 辅助演示快速推进项目 / 先demo快速测试反馈，再开启正式项目

**样式**：编号金色大字（Bebas Neue）· 标题 Playfair Display · 详情 Space Mono · 金色分割线

---

## P10 · 联系页

**section id**：`contact`

**大标题**：
```
[Bebas Neue · 超大]  欢迎来找我玩
[Playfair Display Italic]  我叫陈有米Yuumi，和我的喵喵同名
```

**两列内容**：

| 位置 | 图片 | 说明 |
|------|------|------|
| 左 | `image35.jpeg` | 联系方式 / 二维码 |
| 右 | `image36.png` | 社交平台 / 二维码 |

**样式**：两张图等宽排列，圆角，轻微旋转（Z轴叠加），金色分割线，Space Mono 版权文字

---

## 图片对照总表

| 图片文件 | 用途 | 所在板块 |
|----------|------|----------|
| image1.png | Hero 主视觉大图 | P1-2 |
| image2–5.jpeg | 微信封面图（4张） | P3 微信 |
| image6.jpeg | 抖音主页横版截图 | P3 抖音 |
| image7–10.png | 小红书封面图（4张） | P4 小红书 |
| image11.jpeg | 作品墙全拼图 | P4 作品墙 |
| image12–15.png | AI短链工作流步骤图（4张） | P5 |
| image16.png | AI短链成品封面 + 链接 | P5 |
| image17–19.png | 其他AI图文作品（3张） | P5 |
| image20.jpeg | AI长链工作流步骤图1 | P6 |
| image21–23.png | AI长链工作流步骤图2–4 | P6 |
| image24.png | AI长链成品封面 + 链接 | P6 |
| image25–27.png | 其他AI视频作品（3张） | P6 |
| image28–31.png | 品牌技能配图（4张） | P7-8 |
| image32–34.png | 其他经历品牌logo（3张） | P7-8 |
| image35.jpeg | 联系方式图1 | P10 |
| image36.png | 联系方式图2 | P10 |

---

## 链接汇总

**微信**：
- https://mp.weixin.qq.com/s/nhW3Yp0ckwHWro4tE6qUNg
- https://mp.weixin.qq.com/s/xBoLoW_NHIt1F4dutp5fwQ
- https://mp.weixin.qq.com/s/199hBVE7zpXsEP8_nsLLYg
- https://mp.weixin.qq.com/s/ync3qg83CePAOwD4QCxDVA

**小红书**：
- http://xhslink.com/o/5zeqq9PsaRY（小红书作品1）
- http://xhslink.com/o/6x0MK37o7pF（小红书作品2）
- http://xhslink.com/o/5hZnQCWHrJm（小红书作品3）
- http://xhslink.com/o/50HfShAN2d3（小红书作品4）
- http://xhslink.com/o/41lxGTrPkEL（AI短链成品）
- http://xhslink.com/o/1XsbzJzQfm3（AI图文1）
- http://xhslink.com/o/3zyhraDh6x4（AI图文2）
- http://xhslink.com/o/6BkUFc2Nhde（AI图文3）
- http://xhslink.com/o/3AClNDDK6sH（AI长链成品）
- http://xhslink.com/o/4deR6NjghyO（AI视频1）
- http://xhslink.com/o/6AwFgmVvFfV（AI视频2）
- http://xhslink.com/o/26ANeUwwp4z（AI视频3）

---

## 设计规范备忘（Renaissance UI）

```css
--cream:     #F5F0E8;   /* 主背景 */
--cream-dark:#EDE5D4;   /* 次背景 */
--ink:       #1A1612;   /* 主文字 */
--sepia:     #8B6F4E;   /* 副文字 */
--gold:      #C9A84C;   /* 强调/金线 */
--rust:      #A0522D;   /* 暗部暖色 */
--muted:     #9A8B7A;   /* 标签文字 */

/* 字体 */
/* 大标题：Bebas Neue */
/* 强调斜体：Playfair Display Italic */
/* 标签/数字：Space Mono */

/* 动画 */
/* cubic-bezier(0.32, 0.72, 0, 1) */
/* 入场：translate-y-16 + blur-md + opacity-0 */
/* 悬停：scale(0.98) 物理按压感 */

/* 禁止 */
/* Inter / Roboto / Arial / Helvetica */
/* 对称 Bootstrap 三栏 / 厚边框 / 硬投影 */
```

---

*蓝图版本：v1.0 · 待确认后进入网页制作阶段*
