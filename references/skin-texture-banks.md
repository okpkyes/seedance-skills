# 3D 角色皮肤质感词库 - Skin Texture Banks

本文档收录了 AI 视频/图片中 3D 角色皮肤质感的提示词，解决「假滑、塑料感、动态糊边」等核心痛点。

> 来源参考：CSDN 博客《AI视频3D角色皮肤质感秘籍》（2026年3月）

---

## 使用说明

### 嵌入方法
将对应风格的皮肤质感词叠加在角色主体描述之后，可与表情提示词配合使用。

### 公式结构
```
[角色描述] + [皮肤质感词] + [表情提示词] + [光影风格] + [画质]
```

---

## ⚠️ 绝对不要加的关键词

以下关键词会直接导致皮肤出现「假滑、塑料感」：

| ❌ 禁用词 | 原因 |
|:---------|:----|
| 光滑皮肤 / smooth skin | 导致假滑塑料感 |
| 完美皮肤 / perfect skin | 失去真实肌理层次 |
| 无瑕疵皮肤 / flawless skin | 过度磨皮 |
| 卡通皮肤 / cartoon skin | 风格混淆 |
| 塑料皮肤 / plastic skin | 质感错误 |
| 模糊皮肤 / blurry skin | 低清 |
| 过度磨皮 / over-smoothed | 动态糊边 |
| 极致光滑 / ultra smooth | 动态失真 |
| 假白肤色 / fake white skin | 不自然 |
| 均匀肤色（无层次）/ uniform skin | 失去层次 |

---

## 🎯 通用核心皮肤质感词【必加】

不管什么风格、什么场景，这组核心词是打造真实皮肤的基础：

```
超写实皮肤，细腻毛孔纹理，自然原生肤色，
皮肤轻微油脂光泽，通透肌底感，
面部微泛红肌理，皮肤层次丰富，
光影自然过渡，4K/8K超高清，电影级质感，
PBR物理材质，次表面散射效果，
皮肤细腻不油腻，无磨皮过度感
```

### 英文版
```
hyper-realistic skin, detailed pore texture, natural skin tone,
slight natural sebum glow, translucent skin base,
subtle facial flush texture, rich skin layers,
natural light transition, 4K/8K ultra HD, cinematic quality,
PBR material, subsurface scattering effect,
natural skin texture without over-smoothing
```

---

## 🏯 1. 古风武侠 / 宋代角色｜温润哑光款

**适配场景**：古风剧集、武侠动画、国风3D角色
**核心调性**：温润细腻、哑光高级，贴合东方古典审美，无现代油光感

```
超写实3D古风角色，东方人原生暖调肤色，
细腻哑光皮肤，轻微自然光泽，肌底通透感，
古风温润肤质，高清毛孔纹理，皮肤微泛红，
次表面散射，无塑料感，无油腻感，
4K高清，电影级质感，PBR材质，
面部光影柔和过渡，皮肤纹理自然不突兀
```

### 英文版
```
hyper-realistic 3D ancient Chinese character, warm natural skin tone,
delicate matte skin, subtle natural glow, translucent skin base,
ancient-style warm skin texture, HD pore texture, subtle facial flush,
subsurface scattering, no plastic texture, no oily shine,
4K HD, cinematic quality, PBR material,
soft facial light transition, natural skin texture
```

---

## 👤 2. 现代写实角色｜高清细腻款

**适配场景**：现代都市视频、真人向3D动画、写实系角色创作
**核心调性**：贴近真人肤质，保留自然小瑕疵，光影真实有层次

```
超写实3D现代角色，真实人类皮肤肌理，
高清毛孔细节，T区轻微自然油光，
面部微泛红，皮肤质感层次丰富，
自然原生肤色，可选：皮肤微瑕疵（雀斑/淡痘印），
次表面散射，无塑料假质感，
8K超高清，电影级质感，PBR材质，
光影真实还原，皮肤通透不闷肤
```

### 英文版
```
hyper-realistic 3D modern character, real human skin texture,
HD pore detail, slight natural T-zone shine,
subtle facial flush, rich skin layers,
natural skin tone, optional: subtle skin imperfections (freckles/light acne scars),
subsurface scattering, no plastic texture,
8K ultra HD, cinematic quality, PBR material,
realistic light rendering, translucent skin
```

---

## 🌾 3. 70年代乡村角色｜质朴原生款

**适配场景**：年代剧、乡村题材视频、复古写实3D创作
**核心调性**：质朴粗糙、无过度磨皮，贴合年代场景的原生肤质

```
超写实3D年代角色，质朴哑光皮肤，
轻微原生粗糙纹理，自然黄调肤色，
面部微泛红，乡村真实原生肤质，
无过度光滑感，高清皮肤细节，
次表面散射，4K高清，电影级质感，
PBR材质，光影自然无刻意，
皮肤纹理与场景高度适配
```

### 英文版
```
hyper-realistic 3D period character, rustic matte skin,
slight natural rough texture, natural warm yellow skin tone,
subtle facial flush, rural realistic skin quality,
no over-smoothing, HD skin detail,
subsurface scattering, 4K HD, cinematic quality,
PBR material, natural unforced lighting,
skin texture highly matched to scene
```

---

## 🎬 视频专用｜防糊/防塑料感强化词

做视频和做静态图不同，动态画面容易丢失皮肤细节、出现塑料感。
这组词直接叠加在任意风格提示词后，保障全程肤质一致、细节不丢失：

```
皮肤无塑料感，无光滑假质感，
皮肤细节动态稳定，皮肤纹理不模糊，
光影动态自然过渡，皮肤质感全程统一，
4K动态高清，皮肤细节帧帧清晰，
无动态磨皮，无画面糊边，
肤质与动态动作适配
```

### 英文版
```
no plastic skin texture, no fake smooth texture,
dynamic skin detail stability, skin texture not blurry,
dynamic light transition natural, consistent skin quality throughout,
4K dynamic HD, skin detail clear frame by frame,
no dynamic over-smoothing, no motion blur artifacts,
skin quality matched to dynamic movement
```

---

## 💡 实用技巧

### 1. 按需微调
- 想要淡雀斑效果 → 对应风格词中加入「面部淡雀斑，分布自然」
- 想要无瑕疵清新感 → 去掉「微瑕疵/雀斑/痘印」等词
- 想要更明显的毛孔 → 加入「清晰毛孔细节」

### 2. 分辨率适配
- 短视频场景 → 4K 足够
- 电影级创作 → 选 8K

### 3. 材质强化
**必须保留的关键词**（这是皮肤通透感的核心）：
- `PBR材质` / `PBR material`
- `次表面散射` / `subsurface scattering`

### 4. 风格组合示例
```
[角色描述] + [皮肤质感词] + [表情提示词] + [光影] + [防糊词]
```

示例：
```
古风仙女，身穿汉服广袖，头戴凤冠，
超写实皮肤，细腻哑光毛孔纹理，自然暖调肤色，
表情：温柔微笑，眼含笑意，
金色侧逆光，丁达尔效应，
皮肤细节动态稳定，无动态磨皮，4K动态高清
```

---

## 📊 速查表

| 风格 | 核心关键词 | 适用场景 |
|:----|:----------|:--------|
| 通用核心 | 超写实皮肤、毛孔纹理、次表面散射、PBR | 所有角色 |
| 🏯 古风武侠 | 哑光、温润、东方暖调、无油光 | 古风剧集、国风3D |
| 👤 现代写实 | 高清毛孔、T区油光、微瑕疵 | 都市视频、真人动画 |
| 🌾 70年代乡村 | 质朴、粗糙原生、无过度光滑 | 年代剧、乡村题材 |
| 🎬 视频防糊 | 动态稳定、帧帧清晰、无动态磨皮 | 所有视频（叠加使用） |

---

## 嵌入格式参考

### 图片提示词
```
超写实3D[角色描述]，[皮肤质感词]，[表情]，[光影风格]，[画质]
```

### 视频提示词
```
超写实3D[角色描述]，[皮肤质感词]，[表情]，[动作描述]，
[光影风格]，[画质]，[视频防糊词]
```

### 示例
```
超写实3D古风仙女，东方暖调肤色，细腻哑光皮肤，高清毛孔纹理，
表情：眼神温柔，嘴角带浅笑，
慢慢转头看向镜头，金色逆光，4K动态高清，
皮肤细节帧帧清晰，无动态磨皮，无塑料感
```

---

## 🧬 真人皮肤 6 维平衡表（图生图变换专用）

> 吞噬自 2d-to-realperson-prompt Skill。适用于 2D 动漫 → 真人变换场景，提供比上方 3D 角色皮肤词更精细的真人皮肤控制。

每个维度同时给出**目标状态**和**禁止状态**，消除模糊地带：

| 维度 | 目标状态 | 禁止状态 |
|------|---------|---------|
| **纹理** | 清晰但克制 | 粗糙 / 颗粒过重 |
| **毛孔** | 轻微真实纹理 | 毛孔夸张 |
| **肤色** | 自然、有通透感 | 蜡像感 / 塑料感 |
| **质感** | 细腻、平滑、柔和、有弹性 | 松弛 / 厚重 / 沧桑 |
| **年龄感** | 高质量年轻肌肤 | 成熟粗糙 / 老化感 |
| **后期** | 保留自然明暗起伏 | 过度磨皮 / 过度美颜 / 过度锐化 |

**例外规则：** 除非原角色本身设定明显年龄较大，否则不生成成熟粗糙皮肤。

### 使用方法

将 6 维平衡表作为皮肤描述的**自检清单**：每写一句皮肤描述，对照表格确认目标状态和禁止状态都覆盖到了。

### 与上方 3D 角色皮肤词的区别

| 维度 | 3D 角色皮肤词（上方） | 真人 6 维平衡表（本节） |
|------|---------------------|----------------------|
| 适用 | 3D 渲染角色、AI 漫剧 | 2D→真人图生图变换 |
| 控制 | 词组叠加（PBR/SSS/毛孔） | 维度平衡（目标 vs 禁止） |
| 粒度 | 风格级（古风/现代/乡村） | 参数级（6 维独立控制） |
| 组合 | 选一种风格词组叠加 | 6 维独立检查，按需调整 |

### 真人皮肤核心描述词（配合 6 维平衡表使用）

```
真实摄影级别质感，偏细腻、嫩、干净、自然、有轻微通透感，
皮肤纹理清晰但克制，属于高质量年轻肌肤的真实质感，
细腻、平滑、柔和、富有弹性，保留轻微真实纹理与自然明暗起伏
```
