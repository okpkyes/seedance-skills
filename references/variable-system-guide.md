# 变量系统指南 - Variable System Guide

本文件说明如何在 seedance skill 中使用变量系统，包括变量语法、命名规则、分类和使用示例。

---

## 变量语法

### 标准变量
```
{{variable_name}}
```
- 完全可替换的占位符
- 适用于完全开放的可变参数

示例：
```
{{art_style}}风格的{{character_type}}
```

### 内联默认值
```
{{variable_name: 默认值}}
```
- 有推荐值，但仍可替换
- 适用于有强烈设计意图的核心元素

示例：
```
{{art_style: 赛博朋克}}风格的{{character_type: 赛博少女}}
```

---

## 变量命名规则

### ✅ 好的变量名
- 使用小写英文和下划线
- 描述语义角色，而不是具体值
- 示例：`art_style`、`character_type`、`camera_angle`、`lighting`

### ❌ 坏的变量名
- 使用具体值作为变量名
- 混用大小写或连字符
- 示例：`cyberpunk`、`beautifulGirl`、`camera-angle`

---

## 变量分类

| 类别 | 说明 | 示例 |
|------|------|------|
| `character` | 人物、角色、生物、身体特征、表情 | `character_type`、`hair_style`、`expression` |
| `item` | 服装、道具、配饰、产品、材质 | `outfit`、`accessory`、`weapon` |
| `action` | 动作、姿势、手势、互动 | `action`、`pose`、`gesture` |
| `location` | 地点、场景、背景环境 | `location`、`background` |
| `visual` | 风格、色彩、光影、构图、氛围 | `art_style`、`color_scheme`、`lighting`、`mood` |
| `technical` | 镜头、相机、画幅比例、质量、渲染参数 | `camera_angle`、`shot_type`、`aspect_ratio`、`render_quality` |
| `video` | 视频专属参数 | `video_duration`、`video_style`、`camera_movement` |
| `other` | 其他无法归类的内容 | - |

---

## 使用示例

### 示例 1：简单的变量替换

**提示词模板**：
```
{{character_type}}在{{location}}中，{{action}}，{{art_style}}风格
```

**填充后**：
```
赛博朋克少女在废弃工业区中，奔跑，赛博朋克风格
```

---

### 示例 2：内联默认值

**提示词模板**：
```
{{character_type: 赛博朋克少女}}在{{location: 废弃工业区}}中，
{{action: 奔跑}}，{{art_style: 赛博朋克}}风格，
{{lighting}}，{{camera_angle}}
```

**填充后（使用默认值）**：
```
赛博朋克少女在废弃工业区中，
奔跑，赛博朋克风格，
霓虹灯光，低角度仰拍
```

**填充后（自定义值）**：
```
古风仙子在仙境云海中，
飞行，仙侠国漫风格，
丁达尔光线，俯视鸟瞰
```

---

### 示例 3：视频提示词模板

**提示词模板**：
```
15秒{{video_style}}风格视频，

0-5秒：{{character_type}}在{{location}}中，{{action}}，{{camera_movement}}
5-10秒：{{camera_movement}}，展示{{scene_detail}}
10-15秒：{{ending_action}}，{{mood}}氛围

光照：{{lighting}}
色彩：{{color_scheme}}
画幅：{{aspect_ratio}}

禁止：{{negative_prompt}}
```

**填充后**：
```
15秒电影感风格视频，

0-5秒：赛博朋克少女在废弃工业区中，奔跑，手持跟随
5-10秒：环绕拍摄，展示霓虹灯光和湿地面反射
10-15秒：停下转身，凝视镜头，未来感氛围

光照：霓虹灯光
色彩：赛博紫蓝
画幅：16:9

禁止：文字、水印、Logo
```

---

## 变量提炼流程

当用户提供粗糙提示词或要求变量提炼时，按以下流程处理：

### 1. 识别可变量
- 读取提示词
- 识别可替换的语义单元
- 判断哪些元素应该可变

### 2. 命名变量
- 使用语义角色命名
- 选择合适的变量类别
- 检查是否已有通用变量可复用

### 3. 提供词库建议
- 为重要变量提供 5-12 个候选词组
- 中英双语
- 选项之间语义明显不同

### 4. 输出模板
- 提供变量化后的提示词模板
- 提供填充示例
- 提供词库建议

---

## 质量检查

### 变量使用检查清单
- [ ] 变量名是否描述语义角色（而非具体值）？
- [ ] 变量是否可复用（而非一次性）？
- [ ] 是否过度拆碎（变量太多太细）？
- [ ] 内联默认值是否有意义（而非随意设置）？
- [ ] 词库选项是否足够差异化（5-12个）？

---

## 与 PromptFill 集成

### PromptFill JSON 格式

当用户要求导出为 PromptFill 模板时，使用以下 JSON 格式：

```json
{
  "id": "tpl_descriptive_name",
  "name": { "cn": "中文模板名", "en": "English Template Name" },
  "content": {
    "cn": "{{art_style: 赛博朋克}}风格的{{character_type}}...",
    "en": "{{art_style: Cyberpunk}} style {{character_type}}..."
  },
  "imageUrl": "https://placehold.co/600x400/png?text=Template",
  "selections": {
    "art_style": { "cn": "赛博朋克", "en": "Cyberpunk" }
  },
  "tags": ["人物", "科幻"],
  "language": ["cn", "en"],
  "banks": {
    "art_style": {
      "label": { "cn": "艺术风格", "en": "Art Style" },
      "category": "visual",
      "options": [
        { "cn": "赛博朋克", "en": "Cyberpunk" },
        { "cn": "蒸汽朋克", "en": "Steampunk" }
      ]
    }
  }
}
```

### 规则
- `id` 使用 `tpl_` 前缀
- `content` 支持 `{{variable}}` 和 `{{variable: 默认值}}`
- `selections` 为每个变量提供一个默认值
- `banks` 为变量提供可选词库
- `tags` 描述内容主题，不要把"图片""视频"当作主题标签

---

## 进一步建议

### 何时使用变量系统
- ✅ 用户需要生成多个变体版本
- ✅ 用户需要复用提示词模板
- ✅ 用户要求变量提炼或模板导出
- ❌ 用户只要一次性提示词（不要强迫使用变量）

### 何时省略变量系统
- 用户明确说"只要一句""简单点""不要结构化"
- 提示词非常简单，变量化会过度复杂化
- 用户不需要复用或迭代

---

## 参考资料

- 通用变量词库：`references/universal-variable-banks.md`
- 语汇库：`references/cinematic-vocabulary.md`
- 行业模式库：`references/patterns/`
