# AI人像光影提示词库 - Portrait Lighting Banks

本文档系统整理 AI 人像摄影/视频中的**光影结构提示词**，解决人像光影描述不准确、效果不自然的问题。

> 来源参考：AI人像光影结构教程（小红书/微信公众号）

---

## 使用说明

### 提示词结构公式
按 **「光源方向 + 明暗关系 + 光线质感 + 真实细节 + 反向限制」** 的顺序组合描述，光影层次最清晰。

```
[角色描述] + [光源方向] + [明暗关系] + [光线质感] + [真实细节] + [反向限制]
```

示例：
```
古风女子，自然窗光从左侧45度照射，
脸颊有柔和阴影增加立体感，鼻梁高光突出五官轮廓，
柔和光细腻自然，皮肤有自然反光和发丝高光，
眼神有反射光让眼睛更有神，不要平光不要塑料反光
```

---

## 1. 光源方向（Lighting Direction）

决定光影落点与整体氛围走向。

| 光源方向 | 中文描述 | 英文描述 | 效果特点 |
|---------|:--------|:--------|:--------|
| **自然窗光** | 自然窗光，柔和均匀 | natural window light, soft and even | 柔和均匀，适合清新人像 |
| **侧光** | 侧光，立体有层次 | side lighting, dimensional and layered | 强调面部轮廓，立体感强 |
| **逆光** | 逆光，轮廓光/氛围感 | backlit, rim light / atmospheric glow | 发丝发光，轮廓勾勒，梦幻氛围 |
| **顶光** | 顶光，阴影明显 | top-down lighting, pronounced shadows | 戏剧性阴影，适合高级/暗调风格 |
| **底光** | 底光，恐怖/神秘感 | under lighting from below, dramatic and mysterious | 恐怖片感，神秘氛围 |
| **45度角光** | 45度侧光，经典人像布光 | 45-degree Rembrandt lighting, classic portrait | 经典三角光，人像摄影标准 |
| **伦勃朗光** | 伦勃朗光，三角光 | Rembrandt lighting, triangle of light on cheek | 经典油画感，深邃立体 |
| **蝴蝶光** | 顶光下照，蝴蝶光影 | butterfly / Paramount lighting, light above | 鼻下对称阴影，时尚优雅 |

---

## 2. 明暗关系（Chiaroscuro / Light-Dark Balance）

塑造五官立体感与面部结构。

| 明暗元素 | 中文描述 | 英文描述 | 效果作用 |
|---------|:--------|:--------|:--------|
| **脸颊阴影** | 脸颊有柔和阴影 | soft cheek shadow on one side | 增加面部立体感 |
| **鼻梁高光** | 鼻梁高光突出轮廓 | catchlight on nose bridge, defined nasal contour | 突出鼻梁形态，五官更精致 |
| **眼下暗部** | 眼下自然暗部 | natural shadow under eyes, subtle dark circles | 增强真实感，避免死白 |
| **下颌阴影** | 下颌阴影勾勒轮廓 | jawline shadow, defining facial contour | 优化脸部轮廓，显瘦 |
| **颧骨高光** | 颧骨微微发亮 | subtle highlight on cheekbone | 提升面部高级感 |
| **额头高光** | 额头有自然高光 | natural forehead highlight | 额头饱满，立体感 |
| **颈部过渡** | 颈部自然明暗过渡 | natural neck-to-face light transition | 避免"断头"感，结构完整 |
| **眼窝深邃** | 眼窝有自然阴影 | natural eye socket shadow | 眼睛深邃有神 |

---

## 3. 光线质感（Light Quality）

影响画面氛围与情绪表达。

| 光线质感 | 中文描述 | 英文描述 | 情绪氛围 |
|---------|:--------|:--------|:--------|
| **柔和光** | 柔和光，细腻自然 | soft diffused light, gentle and natural | 清新、温柔、自然 |
| **硬光** | 硬光，对比强烈 | hard direct light, strong contrast | 硬朗、戏剧性、时尚 |
| **暖光** | 暖光，温暖治愈 | warm golden light, cozy and healing | 温暖、治愈、回忆 |
| **冷光** | 冷光，清冷高级 | cool blue light, crisp and sophisticated | 冷冽、高级、科技感 |
| **自然光** | 自然光，清透 | natural daylight, clear and airy | 通透、真实、日常 |
| **魔幻光** | 魔幻光，梦幻 | magical ethereal light, dreamy and surreal | 仙侠、梦幻、超现实 |
| **单束光** | 单束光，戏剧性 | single beam of light, dramatic spotlight effect | 舞台感、神秘、聚焦 |
| **漫射光** | 漫射光，朦胧 | diffused ambient light, hazy and atmospheric | 朦胧、艺术、情绪 |
| **体积光** | 体积光，丁达尔效应 | volumetric light beams, Tyndall effect | 神圣、仙境、电影感 |
| **霓虹光** | 霓虹光，赛博感 | neon colored light, cyberpunk vibe | 赛博、未来、都市 |

---

## 4. 真实细节（Realistic Details）

提升真实感与细节可信度。

| 真实细节 | 中文描述 | 英文描述 | 效果作用 |
|---------|:--------|:--------|:--------|
| **皮肤反光** | 皮肤有自然反光，自然油光感 | natural skin reflection, subtle sheen on skin | 真实皮肤质感，避免假面 |
| **发丝高光** | 发丝有细腻光泽感 | hair with delicate highlight strands, silky shine | 头发有生命感，不僵硬 |
| **眼神反光** | 眼神有反射光，让眼睛更有神 | eye light catchlight, reflective glint in eyes | 眼睛有神，不空洞 |
| **衣料受光** | 衣料有自然受光变化，体现材质与光向 | fabric catches light naturally, showing material texture | 衣服有材质感，不贴图 |
| **睫毛投影** | 睫毛在下眼睑有自然投影 | natural eyelash shadow on lower lid | 极致真实感 |
| **毛孔可见** | 皮肤毛孔细腻可见 | visible fine pores on skin | 超高真实度 |
| **唇面高光** | 嘴唇有自然高光 | natural lip highlight, moist and glossy | 嘴唇饱满自然 |
| **耳廓透光** | 耳廓微微透光 | subtle ear translucency, sss effect | 次表面散射，耳朵真实 |
| **边缘光** | 人物轮廓边缘有微弱光晕 | subtle rim light on subject edge | 人物与背景分离，层次分明 |

---

## 5. 反向限制（Negative Constraints）

排除常见问题，避免翻车效果。

| 问题 | 中文描述 | 英文描述 | 后果 |
|:-----|:--------|:--------|:----|
| **不要平光** | 不要平光，缺乏立体感 | no flat lighting, avoid flat on-face light | 面部像饼，毫无层次 |
| **不要过曝** | 不要过曝，细节丢失 | no overexposure, preserve highlight details | 亮部死白，无细节 |
| **不要塑料反光** | 不要塑料反光，假亮不自然 | no plastic-like reflection, avoid unnatural shine | 皮肤像塑料/蜡像 |
| **不要死黑阴影** | 不要死黑阴影，压抑脏乱 | no crushed black shadows, avoid muddy dark areas | 暗部无细节，画面脏 |
| **不要油光满面** | 不要油光满面，油腻 | no excessive oil shine, avoid greasy face | 皮肤泛油光，不高级 |
| **不要硬边阴影** | 不要硬边阴影，不自然 | no harsh edged shadows, natural soft shadow falloff | 阴影像贴图，假 |
| **不要色偏** | 不要色偏，肤色正常 | no color cast, natural skin color accuracy | 肤色发绿/发紫 |
| **不要眼神无光** | 不要眼神无光，死鱼眼 | no dead eyes, ensure catchlight in pupils | 眼睛像盲人，无生气 |
| **不要背景过亮** | 不要背景过亮抢主体 | no overbright background competing with subject | 主体被背景淹没 |
| **不要光斑过散** | 不要光斑过散，分散注意力 | no distracting scattered light spots | 画面杂乱 |

---

## 6. 组合光影公式（直接复制使用）

### 6.1 清新自然人像
```
自然窗光，柔和均匀，脸颊有柔和阴影增加立体感，
鼻梁高光突出五官，柔和光细腻自然，皮肤有自然反光和眼神反光，
不要平光，不要过曝，不要塑料反光
```

### 6.2 高级感时尚人像
```
侧光，伦勃朗光，45度角照射，脸颊阴影立体，
鼻梁高光精致，下颌阴影勾勒轮廓，硬光对比强烈，
发丝高光细腻，皮肤有质感反光，眼神有光，
不要平光，不要死黑阴影，不要塑料反光
```

### 6.3 梦幻逆光人像
```
逆光，轮廓光氛围感，金色体积光丁达尔效应，
发丝逆光发光，柔和边缘光勾勒人物，
皮肤自然透光感，眼神有反射光，
不要过曝，不要死黑阴影，不要背景过亮
```

### 6.4 赛博朋克人像
```
霓虹冷光，紫蓝+粉色双色打光，侧光立体有层次，
鼻梁和颧骨有锐利高光，硬光对比强烈，
皮肤有微妙反光，眼神有霓虹反射光，
不要平光，不要色偏，不要油光满面
```

### 6.5 古风仙气人像
```
魔幻光，体积光丁达尔效应，逆光氛围感，
柔和光细腻自然，皮肤有自然透光和微微高光，
发丝有柔和光泽，眼神有神仙光，衣料自然受光，
不要平光，不要死黑阴影，不要塑料反光
```

### 6.6 暗调电影感人像
```
单束光，戏剧性，顶光阴影明显，脸颊和眼窝有深邃阴影，
鼻梁和颧骨有焦点高光，硬光对比强烈，
皮肤有真实质感，眼神有微弱反光，
不要过曝，不要油光，不要塑料反光
```

---

## 7. 视频专用光影（动态稳定）

视频中人像光影需要动态过程中保持一致，额外增加：

```
光影动态稳定，阴影边缘自然过渡，
皮肤反光帧帧一致，眼神光位置稳定，
发丝高光随动作自然变化，不要光影闪烁，不要阴影跳动
```

---

## 8. 中英文对照速查表

| 中文 | English | 适用场景 |
|:-----|:--------|:--------|
| 自然窗光 | natural window light | 清新日常 |
| 侧光/伦勃朗光 | side light / Rembrandt lighting | 时尚人像 |
| 逆光/轮廓光 | backlit / rim light | 梦幻氛围 |
| 顶光 | top-down lighting | 暗调戏剧 |
| 体积光/丁达尔 | volumetric light / Tyndall effect | 仙侠/神圣 |
| 霓虹光 | neon colored light | 赛博朋克 |
| 柔和光 | soft diffused light | 温柔治愈 |
| 硬光 | hard direct light | 时尚硬朗 |
| 暖光 | warm golden light | 温暖回忆 |
| 冷光 | cool blue light | 清冷高级 |
| 脸颊阴影 | cheek shadow | 立体感 |
| 鼻梁高光 | nose bridge highlight | 精致五官 |
| 眼神反光 | eye catchlight | 眼睛有神 |
| 发丝高光 | hair highlight | 头发质感 |
| 皮肤反光 | skin reflection | 真实质感 |
| 不要平光 | no flat lighting | 避免饼脸 |
| 不要过曝 | no overexposure | 保留细节 |
| 不要塑料反光 | no plastic reflection | 避免假面 |
| 不要死黑阴影 | no crushed blacks | 避免脏暗 |

---

## 9. 提示词嵌入格式

### 图片提示词
```
[角色描述] + [光源方向] + [明暗关系] + [光线质感] + [真实细节] + [反向限制] + [画质]
```

### 视频提示词
```
[角色描述] + [光源方向] + [明暗关系] + [光线质感] + [真实细节] + [动态光影稳定] + [反向限制] + [画质]
```

### 完整示例
```
古风女子，自然窗光从左侧45度照射，
脸颊有柔和阴影增加立体感，鼻梁高光突出五官轮廓，
柔和光细腻自然，皮肤有自然反光和发丝高光，
眼神有反射光让眼睛更有神，衣料自然受光，
光影动态稳定，不要平光，不要过曝，不要塑料反光，
4K高清，电影级质感，写实风格
```
