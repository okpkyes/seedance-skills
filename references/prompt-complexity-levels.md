# 提示词复杂度系统 - Prompt Complexity Levels

本文件说明 seedance skill 中的三层提示词复杂度系统，包括极简版、平衡版和结构化版的使用场景和格式。

---

## 概述

提示词复杂度分为三个级别，根据用户需求和场景选择合适的级别：

| 级别 | 名称 | 适用场景 | 输出格式 |
|------|------|---------|---------|
| Level 1 | 极简版 | 快速试图、不喜欢复杂结构 | 一句话或简短段落 |
| Level 2 | 平衡版 | 大多数用户（默认推荐） | 逗号分隔的关键词列表 |
| Level 3 | 结构化版 | 精细控制、商业级、可复用 | 分组标注的完整描述 |

---

## Level 1：极简版（Minimal）

### 适用场景
- 用户要求"只要一句""简单点"
- 快速试图、测试想法
- 不喜欢复杂结构的用户
- 社交媒体快速生成（如抖音、快手）

### 格式
```
[主体]，[核心风格]，[主要场景/构图]，[光影或氛围]，[质量/风格收尾]
```

### 示例

**视频提示词（极简版）**：
```
赛博朋克少女在雨夜街道奔跑，霓虹灯光，电影感，高清
```

**图片提示词（极简版）**：
```
A cyberpunk girl in a rainy neon alley, cinematic lighting, high-detail portrait, shallow depth of field
```

### 注意事项
- 保持简洁，不要超过 2 行
- 只保留最核心的元素
- 适合快速复制粘贴

---

## Level 2：平衡版（Balanced）

### 适用场景
- 大多数用户的默认选择
- 需要一定控制，但不想太复杂
- 适合即梦、可灵等视频平台
- 适合 Midjourney、Stable Diffusion 等图像平台

### 格式
```
[主体和关键特征], [环境], [动作或姿态], [构图/镜头], [光影], [色彩], [风格], [质量细节], [画幅比例（如适用）]
```

### 示例

**视频提示词（平衡版）**：
```
赛博朋克少女，穿着发光皮衣，在雨夜街道奔跑，
低角度跟随拍摄，霓虹灯光在湿地面反射，
紫蓝冷色调，电影感，高清，16:9
```

**图片提示词（平衡版）**：
```
A cyberpunk girl in glowing leather jacket, running on a rainy night street,
low angle follow shot, neon lights reflecting on wet ground,
cyber purple-blue color tone, cinematic lighting, high detail, 16:9
```

### 注意事项
-  comma 分隔，关键词清晰
- 包含主要维度，但不必面面俱到
- 适合大多数生成场景

---

## Level 3：结构化版（Structured）

### 适用场景
- 用户要求高级、模板化、商业级
- 需要精细控制每个维度
- 可复用、可迭代
- 适合广告、电影、专业创作

### 格式
```markdown
[主体]：...
[场景]：...
[构图]：...
[光影]：...
[色彩]：...
[风格]：...
[细节]：...
[质量]：...
[负面约束]：...
```

### 示例

**视频提示词（结构化版）**：
```
主体：赛博朋克少女，银白短发，机械义肢，冷漠表情
场景：雨夜的赛博朋克都市街道，霓虹招牌，湿地面反射
构图：低角度仰拍，手持跟随，浅景深
光影：霓虹灯光为主，蓝紫冷调，偶尔暖橙反光
色彩：赛博紫蓝为主，小面积暖橙对比
风格：电影感，科幻写实，未来感
细节：雨滴、水面反射、皮肤纹理、服装材质
质量：8K，电影级渲染，光线追踪
负面约束：文字、水印、Logo、变形、闪烁
```

**图片提示词（结构化版）**：
```
Subject: A cyberpunk girl with silver short hair, mechanical prosthetics, cold expression
Scene: Rainy night cyberpunk city street, neon signs, wet ground reflections
Composition: Low angle shot, hand-held follow, shallow depth of field
Lighting: Neon lighting, cyber purple-blue tones, occasional warm orange reflections
Color: Cyber purple-blue dominant, small warm orange accents
Style: Cinematic, sci-fi photorealistic, futuristic
Details: Rain drops, water reflections, skin texture, clothing material
Quality: 8K, cinematic render, ray tracing
Negative constraints: text, watermark, logo, deformation, flickering
```

### 注意事项
- 每个维度单独标注，清晰易读
- 适合精细控制和迭代
- 可作为模板复用

---

## 视频专属：时间戳分镜法

对于视频提示词，Level 2 和 Level 3 可以使用时间戳分镜法：

### 格式
```
[总时长][视频风格]视频，

0-[t1]秒：[镜头/动作/场景]，[细节]
[t1]-[t2]秒：[镜头/动作/场景]，[细节]
[t2]-[t3]秒：[镜头/动作/场景]，[细节]

光照：[光照描述]
色彩：[色彩描述]
音效：[音效描述]
禁止：[负面约束]
```

### 示例
```
15秒电影感视频，

0-5秒：低角度特写，赛博朋克少女在雨中行走，霓虹灯光打在脸上
5-10秒：手持跟随，少女奔跑，镜头晃动感，湿地面反射
10-15秒：环绕拍摄，少女停下转身，凝视镜头，未来感氛围

光照：霓虹灯光，体积光
色彩：赛博紫蓝，暖橙对比
音效：电子乐，雨声，脚步声
禁止：文字、水印、Logo
```

---

## 如何选择复杂度级别

### 判断流程

1. **用户明确说"只要一句""简单点"** → Level 1（极简版）
2. **用户没有明确要求** → Level 2（平衡版，默认）
3. **用户要求"高级""专业""结构化""模板"** → Level 3（结构化版）
4. **视频超过 15 秒，需要分镜** → Level 2 或 Level 3 + 时间戳分镜

### 输出策略

大多数情况下，输出两个版本：
- **极简增强版**（Level 1 或 Level 2）
- **高级结构化版**（Level 3）

让用户根据自己的需求选择。

---

## 质量检查清单

### Level 1（极简版）
- [ ] 是否足够简洁（≤2行）？
- [ ] 是否保留最核心的元素？
- [ ] 是否适合快速复制？

### Level 2（平衡版）
- [ ] 是否包含所有重要维度？
- [ ] 是否 comma 分隔，清晰易读？
- [ ] 是否适合大多数生成场景？

### Level 3（结构化版）
- [ ] 每个维度是否单独标注？
- [ ] 是否适合精细控制？
- [ ] 是否可作为模板复用？

---

## 进一步优化建议

在输出提示词后，可以给出进一步优化建议：

- 询问是否需要针对特定平台（即梦、可灵、Midjourney、SD）微调
- 建议画幅比例、风格变体或镜头变体
- 建议添加负面提示词（如平台支持）
- 建议转换为模板或变量化（如需复用）

---

## 参考资料

- 变量系统指南：`references/variable-system-guide.md`
- 通用变量词库：`references/universal-variable-banks.md`
- 语汇库：`references/cinematic-vocabulary.md`
