# 图像反推提示词指南 - Image To Prompt Guide

本文件说明如何使用 seedance skill 从参考图片生成视频或图像提示词。

---

## 功能说明

**图像反推提示词**（Image To Prompt）是指从参考图片中提取关键视觉要素，生成可用于 AI 生成工具的高质量提示词。

适用场景：
- 用户上传、链接或引用一张图片
- 用户说"反推提示词""图生文""看图写提示词""img2prompt"
- 用户只有参考图，但想生成提示词或可复用模板

---

## 处理流程

### 1. 观察画面要素

从以下维度观察图片：

**核心要素**：
- `subject`：主体（人物、产品、物体、生物）
- `action`：动作、姿势、行为、互动
- `scene`：场景、背景、环境

**视觉控制**：
- `composition`：构图、画面布局
- `camera_angle`：视角（平视、低角度、俯视、特写等）
- `lighting`：光照（影棚柔光、霓虹灯光、黄金时刻等）
- `color_scheme`：色彩方案（莫兰迪、暖调、冷调等）
- `mood`：情绪氛围（宁静、戏剧化、未来感等）

**风格与质量**：
- `style`：视觉风格（赛博朋克、水墨、胶片感等）
- `material`：材质（玻璃、金属、布料等）
- `render_quality`：渲染质量（照片写实、8K、电影级等）

**其他**：
- `text`：图片中的文字（如有）
- `aspect_ratio`：画幅比例（1:1、16:9、9:16等）

### 2. 区分高置信观察和推测性风格词

**高置信观察**：
- 直接可见的元素（主体、颜色、构图、光照等）
- 可以明确描述的要素

**推测性风格词**：
- 基于画面感觉推断的风格（如"电影感""复古胶片感"）
- 需要标注为"可能""推测"的风格词

### 3. 输出提示词

至少输出一个可直接使用的提示词，建议提供两个版本：
- **极简增强版**（Level 1 或 2）
- **高级结构化版**（Level 3）

### 4. 可选：生成模板或变量

如果用户还需要可复用的模板，进入变量提炼流程。

---

## 输出模板

### 标准输出格式

```markdown
## 图像提示词

### 极简增强版
[Level 1 或 Level 2 提示词]

### 高级结构化版
[Level 3 提示词]

### 画面要素
- 主体：[观察到的主体]
- 场景：[观察到的场景]
- 构图：[观察到的构图]
- 光影：[观察到的光照]
- 色彩：[观察到的色彩]
- 风格：[观察到的风格]

### 进一步建议
- [具体、可执行的建议]
```

---

## 示例

### 示例 1：产品摄影图片

**用户输入**：
```
请根据这张产品图片反推提示词：
[图片： luxury perfume bottle on cream background]
```

**建议输出**：
```markdown
## 图像提示词

### 极简增强版
Luxury perfume bottle on cream background, soft studio lighting, elegant commercial photography, high-detail product shot

### 高级结构化版
Subject: A luxury glass perfume bottle with refined label and transparent golden liquid
Scene: Clean cream-colored studio background with soft geometric display blocks
Composition: Centered product hero shot, low front angle, balanced negative space for ad copy
Lighting: Diffused studio softbox lighting with gentle rim highlights and subtle reflections
Color: Warm cream, champagne gold, pale blush accents
Material: Clear glass, glossy cap, soft paper label
Style: Premium commercial product photography, minimalist luxury advertising
Quality: Ultra-clean, high-resolution, realistic reflections, polished editorial finish

### 画面要素
- 主体：香水瓶
- 场景：影棚产品布景
- 构图：居中产品特写，低角度前拍
- 光影：柔和影棚布光，边缘高光
- 色彩：暖奶油色、香槟金、淡粉色调
- 风格：奢华极简产品广告

### 进一步建议
- 如果用于即梦视频，可生成 10 秒产品展示视频，添加缓慢旋转和光照变化
- 如果用于电商主图，建议保留更干净的背景和更少装饰
- 画幅比例建议：1:1（方图）或 4:5（竖版）
```

---

### 示例 2：赛博朋克角色图片

**用户输入**：
```
根据这张赛博朋克少女的图片，反推视频提示词：
[图片：cyberpunk girl in neon alley]
```

**建议输出**：
```markdown
## 视频提示词

### 极简增强版
15秒视频，赛博朋克少女在霓虹街道行走，低角度跟随，电影感，霓虹灯光

### 高级结构化版
15秒赛博朋克风格视频，

0-5秒：低角度特写，赛博朋克少女在雨中行走，霓虹灯光打在脸上，冷峻表情
5-10秒：手持跟随，少女走过霓虹招牌下，镜头晃动感，湿地面反射
10-15秒：侧面跟拍，少女停下，转头凝视镜头，未来感氛围

主体：赛博朋克少女，银白短发，机械义肢，冷峻表情
场景：雨夜赛博朋克街道，霓虹招牌，湿地面反射
构图：低角度、手持跟随、侧面跟拍
光照：霓虹灯光为主，蓝紫冷调，偶尔暖橙反光
色彩：赛博紫蓝为主，小面积暖橙对比
风格：电影感，科幻写实，未来感
质量：8K，电影级渲染
音效：电子乐，雨声，脚步声
禁止：文字、水印、Logo、变形

### 画面要素
- 主体：赛博朋克少女
- 场景：雨夜霓虹街道
- 构图：低角度、跟随镜头
- 光影：霓虹灯光
- 色彩：紫蓝冷调
- 风格：赛博朋克、电影感

### 进一步建议
- 可添加参考图片：@图片1（人物外观）、@图片2（场景氛围）
- 如使用即梦平台，可生成 15 秒视频，分 3 个镜头
- 可尝试不同镜头运动：环绕拍摄、无人机俯拍
```

---

## 注意事项

### 重要声明
- **不要声称可以还原图片的原始隐藏参数**
- 应说明这是对画面的实用重构
- 提示词是基于观察的推测，不是原始生成参数

### 质量检查
- 提示词是否有清晰主体？
- 是否区分了高置信观察和推测性风格词？
- 提示词是否可直接使用？
- 是否提供了进一步建议？

---

## 视频反推特殊说明

当用户从图片生成**视频提示词**时，需要额外考虑：

### 1. 添加时间维度
- 图片是静态的，视频需要动态
- 推断可能的动作或镜头运动

### 2. 分镜设计
- 如果视频超过 10 秒，建议使用时间戳分镜法
- 每个镜头 3-5 秒

### 3. 参考素材
- 图片可作为 @引用素材
- 可添加其他参考图片（如动作参考、场景参考）

### 4. 平台适配
- 即梦：支持图片参考，可上传参考图
- 可灵：支持图片参考，可生成图片转动画
- Runway: 支持 Image To Video

---

## 参考资料

- 提示词复杂度系统：`references/prompt-complexity-levels.md`
- 变量系统指南：`references/variable-system-guide.md`
- 通用变量词库：`references/universal-variable-banks.md`
