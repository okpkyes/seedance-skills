# 通用变量词库 - Universal Variable Banks

本文件收录了常见 AI 提示词场景下的通用变量，供 seedance skill 自动匹配复用。

> 扩展词库时，优先检查此文件是否已有可复用的变量，再决定是否新建。

---

## 使用说明

### 变量语法
- 标准变量：`{{variable_name}}`
- 内联默认值：`{{variable_name: 默认值}}`

### 变量命名规则
- 使用小写英文和下划线
- 变量名描述语义角色，而不是具体值
- 好例子：`art_style`、`character_type`、`camera_angle`
- 坏例子：`cyberpunk`、`beautifulGirl`、`camera-angle`

### 变量分类
- `character`：人物、角色、生物、身体特征、表情
- `item`：服装、道具、配饰、产品、材质
- `action`：动作、姿势、手势、互动
- `location`：地点、场景、背景环境
- `visual`：风格、色彩、光影、构图、氛围
- `technical`：镜头、相机、画幅比例、质量、渲染参数
- `other`：其他无法归类的内容

---

## 视觉风格类 (visual)

### `art_style` — 艺术风格

| 中文 | English |
|------|---------|
| 赛博朋克 | Cyberpunk |
| 蒸汽朋克 | Steampunk |
| 水墨国风 | Chinese Ink Painting |
| 吉卜力风格 | Ghibli Studio Style |
| 超现实主义 | Surrealism |
| 暗黑哥特 | Dark Gothic |
| 赛博道家 | Cyber-Taoist |
| 新海诚风格 | Makoto Shinkai Style |
| 复古胶片 | Vintage Film |
| 极简主义 | Minimalism |
| 波普艺术 | Pop Art |
| 仙侠国漫 | Chinese Xianxia Animation |
| 3D 写实渲染 | Photorealistic 3D Render |
| 像素艺术 | Pixel Art |
| 王家卫风格 | Wong Kar-wai Style |
| 诺兰风格 | Christopher Nolan Style |
| 大卫·芬奇风格 | David Fincher Style |

---

### `color_scheme` — 色彩方案

| 中文 | English |
|------|---------|
| 霓虹冷色调 | Neon Cool Tones |
| 金红暖色调 | Gold-Red Warm Tones |
| 莫兰迪灰调 | Morandi Muted Tones |
| 马卡龙粉彩 | Pastel Macaron Colors |
| 黑白高对比 | High-Contrast Black & White |
| 赛博紫蓝 | Cyber Purple-Blue |
| 森系绿调 | Forest Green Tones |
| 日落橘粉 | Sunset Orange-Pink |
| 深海蓝绿 | Deep Ocean Teal |
| 复古棕褐 | Vintage Sepia |
| 电影感暖调 | Cinematic Warm Tones |
| 科技冷蓝 | Tech Cold Blue |

---

### `lighting` — 光照效果

| 中文 | English |
|------|---------|
| 霓虹灯光 | Neon Lighting |
| 丁达尔光线 | Tyndall Effect Rays |
| 黄金时刻光 | Golden Hour Light |
| 影棚三点布光 | Studio Three-Point Lighting |
| 月光冷光 | Moonlight Cold Glow |
| 逆光剪影 | Backlight Silhouette |
| 篝火暖光 | Campfire Warm Glow |
| 荧光生物光 | Bioluminescent Glow |
| 电影感打光 | Cinematic Lighting |
| 漫射柔光 | Diffused Soft Light |
| 体积光束 | Volumetric Light Beams |
| 赛博朋克霓虹 | Cyberpunk Neon Glow |
| 阴雨天光 | Overcast Daylight |

---

### `mood` — 情绪氛围

| 中文 | English |
|------|---------|
| 史诗宏大 | Epic and Grand |
| 宁静祥和 | Calm and Serene |
| 神秘莫测 | Mysterious and Enigmatic |
| 热血沸腾 | Intense and Thrilling |
| 忧郁诗意 | Melancholic and Poetic |
| 梦幻飘渺 | Dreamy and Ethereal |
| 黑暗压抑 | Dark and Oppressive |
| 温暖治愈 | Warm and Healing |
| 孤独苍凉 | Solitary and Desolate |
| 活泼欢快 | Lively and Cheerful |
| 未来感 | Futuristic |
| 复古怀旧 | Nostalgic |
| 奢华高级 | Luxurious |
| 恐怖惊悚 | Horror and Thriller |

---

## 主体角色类 (character)

### `character_type` — 角色类型

| 中文 | English |
|------|---------|
| 赛博少女 | Cyberpunk Girl |
| 古风仙子 | Ancient Fantasy Fairy |
| 机甲战士 | Mecha Warrior |
| 精灵弓手 | Elf Archer |
| 暗影刺客 | Shadow Assassin |
| 魔法师 | Mage |
| 剑修 | Sword Cultivator |
| 龙族王子 | Dragon Prince |
| 末日幸存者 | Post-Apocalypse Survivor |
| 星际探索者 | Interstellar Explorer |
| 霸道总裁 | Overbearing CEO |
| 古风侠客 | Ancient Martial Hero |
| 现代都市青年 | Modern Urban Youth |
| 悬疑侦探 | Mystery Detective |

---

### `hair_style` — 发型

| 中文 | English |
|------|---------|
| 长直黑发 | Long Straight Black Hair |
| 双马尾 | Twin Tails |
| 银白短发 | Silver White Short Hair |
| 蓬松卷发 | Fluffy Curly Hair |
| 丸子头 | Bun Hairstyle |
| 渐变染发 | Gradient Dyed Hair |
| 半扎发 | Half-Up Half-Down |
| 辫子发型 | Braided Hair |

---

### `expression` — 表情神态

| 中文 | English |
|------|---------|
| 冷漠淡然 | Cold and Indifferent |
| 温柔微笑 | Gentle Smile |
| 霸气凛然 | Domineering Presence |
| 忧郁沉思 | Melancholic Contemplation |
| 俏皮可爱 | Playful and Cute |
| 坚定执着 | Determined and Resolute |
| 慵懒慵懒 | Lazy and Languid |
| 惊喜雀跃 | Surprised and Delighted |

---

## 服装道具类 (item)

### `outfit` — 服装风格

| 中文 | English |
|------|---------|
| 汉服广袖 | Hanfu Wide Sleeves |
| 赛博皮衣 | Cyberpunk Leather Jacket |
| 战甲盔甲 | Battle Armor |
| 道袍仙衣 | Taoist Robe |
| 学院制服 | School Uniform |
| 晚礼服 | Evening Gown |
| 街头潮服 | Streetwear |
| 古罗马长袍 | Ancient Roman Toga |
| 机甲战衣 | Mecha Suit |
| 霸总西装 | CEO Suit |
| 古风侠客装 | Ancient Martial Hero Outfit |
| 现代休闲装 | Modern Casual Wear |

---

### `accessory` — 配饰

| 中文 | English |
|------|---------|
| 耳机发光 | Glowing Headphones |
| 古典发簪 | Classical Hairpin |
| 机械义肢 | Mechanical Prosthetics |
| 护目镜 | Goggles |
| 羽毛披风 | Feathered Cape |
| 符文项链 | Runic Necklace |
| 全息投影腕带 | Holographic Wristband |
| 战术腰包 | Tactical Waist Bag |

---

### `weapon` — 武器/道具

| 中文 | English |
|------|---------|
| 符文长剑 | Runic Longsword |
| 光子步枪 | Photon Rifle |
| 魔法权杖 | Magic Staff |
| 双刃战斧 | Double-Bladed Battleaxe |
| 弓弩 | Crossbow |
| 飞镖暗器 | Throwing Darts |
| 能量护盾 | Energy Shield |
| 时空镰刀 | Time-Space Scythe |

---

## 场景环境类 (location)

### `location` — 场景地点

| 中文 | English |
|------|---------|
| 赛博朋克都市 | Cyberpunk Metropolis |
| 古风江南水乡 | Ancient Jiangnan Water Town |
| 外太空星际 | Outer Space |
| 废弃工业区 | Abandoned Industrial Zone |
| 魔法学院 | Magic Academy |
| 深海珊瑚礁 | Deep-Sea Coral Reef |
| 熔岩火山口 | Lava Volcano Crater |
| 仙境云海 | Fairyland Cloud Sea |
| 赛博酒吧 | Cyberpunk Bar |
| 雪山之巅 | Mountain Summit |
| 樱花古道 | Cherry Blossom Path |
| 末日废土 | Post-Apocalyptic Wasteland |
| 现代都市街道 | Modern Urban Street |
| 古代宫殿 | Ancient Palace |
| 办公室 | Office |
| 咖啡馆 | Cafe |

---

### `background` — 背景环境

| 中文 | English |
|------|---------|
| 渐变纯色 | Gradient Solid Color |
| 虚化散景 | Bokeh Background |
| 星空银河 | Starry Galaxy |
| 城市霓虹 | City Neon Lights |
| 自然森林 | Natural Forest |
| 抽象几何 | Abstract Geometric |
| 烟雾弥漫 | Misty Fog |
| 水面倒影 | Water Reflection |

---

## 摄影技术类 (technical)

### `camera_angle` — 构图视角

| 中文 | English |
|------|---------|
| 低角度仰拍 | Low Angle Shot |
| 俯视鸟瞰 | Bird's Eye View |
| 平视正面 | Eye-Level Front |
| 侧面轮廓 | Side Profile |
| 斜45度 | 45-Degree Angle |
| 特写近景 | Close-Up Shot |
| 全身远景 | Full Body Long Shot |
| 3/4 侧面 | Three-Quarter View |

---

### `shot_type` — 景别

| 中文 | English |
|------|---------|
| 大远景 | Extreme Long Shot |
| 远景 | Long Shot |
| 全景 | Full Shot |
| 中景 | Medium Shot |
| 近景 | Medium Close-Up |
| 特写 | Close-Up |
| 大特写 | Extreme Close-Up |
| 过肩镜头 | Over-the-Shoulder Shot |

---

### `camera_movement` — 镜头运动（视频专属）

| 中文 | English |
|------|---------|
| 固定镜头 | Static Shot |
| 平移跟随 | Pan Follow |
| 推拉镜头 | Dolly Zoom |
| 手持晃动 | Handheld Shaky |
| 环绕拍摄 | Orbit Shot |
| 无人机俯拍 | Drone Top-Down |
| 第一人称 | First-Person POV |
| 滑动轨道 | Slider Shot |

---

### `render_quality` — 渲染质量

| 中文 | English |
|------|---------|
| 超高精细度 | Ultra-High Detail |
| 8K 分辨率 | 8K Resolution |
| 电影级渲染 | Cinematic Render |
| 光线追踪 | Ray Tracing |
| 大师级杰作 | Masterpiece Quality |
| 专业摄影级 | Professional Photography |
| 概念艺术级 | Concept Art Quality |

---

### `aspect_ratio` — 画幅比例

| 中文 | English |
|------|---------|
| 1:1 方图 | 1:1 Square |
| 16:9 宽屏 | 16:9 Widescreen |
| 9:16 竖屏 | 9:16 Vertical |
| 4:3 标准 | 4:3 Standard |
| 2:3 竖幅 | 2:3 Portrait |
| 3:2 横幅 | 3:2 Landscape |
| 21:9 超宽 | 21:9 Ultrawide |

---

## 视频专属类 (video)

### `video_duration` — 视频时长

| 选项 | 说明 |
|------|------|
| 5秒 | 极短，适合测试 |
| 10秒 | 短片段 |
| 15秒 | 标准短视频 |
| 30秒 | 中等长度 |
| 60秒 | 长视频 |

---

### `video_style` — 视频风格

| 中文 | English |
|------|---------|
| 电影感 | Cinematic |
| 广告片 | Commercial |
| 纪录片 | Documentary |
| 音乐MV | Music Video |
| 短视频 | Short Video |
| 直播感 | Live Stream Style |

---

### `storyboard_structure` — 分镜结构

| 中文 | English |
|------|---------|
| 单镜头 | Single Shot |
| 两镜头 | Two-Shot Structure |
| 三镜头 | Three-Shot Structure |
| 多镜头 | Multi-Shot Structure |
| 时间戳分镜 | Timestamped Storyboard |

---

## 扩展说明

### 新建变量的判断标准

| 条件 | 建议 |
|------|------|
| 该变量在多种提示词中普遍出现 | ✅ 建议新建并加入词库 |
| 词库选项具有明显差异性（5个以上） | ✅ 适合独立词库 |
| 变量高度场景专属（仅一个模板用） | ⚠️ 考虑内联默认值 `{{key: 值}}` |
| 选项不到3个且含义相近 | ❌ 不建议独立词库，合并到相近变量 |

### 词库质量标准

- **选项数量**：5–12 个为最佳
- **差异度**：每个选项之间语义明显不同
- **双语完整**：每个词条必须有中英文
- **英文质量**：使用 AI 平台主流描述词，不机械翻译

---

## 使用建议

### 何时使用变量
- 用户需要复用、替换、选择或做模板时
- 提示词中有明显可变的语义单元
- 需要生成多个变体版本时

### 何时使用内联默认值
- 有强烈设计意图的核心元素
- 完全开放的可变参数 → 使用普通占位
- 临时性、场景专属的词条 → 使用内联默认值（无需建词库）

示例：
```
# 普通占位（完全可替换）
{{art_style}}风格的{{character_type}}

# 内联默认值（有推荐值，但可替换）
{{art_style: 赛博朋克}}风格的{{character_type: 赛博少女}}
```
