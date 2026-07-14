# 人物真实感（去 AI 感·电影级写实）

生图最常踩的"假滑塑料感"陷阱的解药：电影级写实人像锚点 + 反向约束清单。

## 完整提示词

```
电影级写实人像，真实活人质感，去除AI感，

场景包含体积光（Volumetric light）、空气悬浮微粒，

带有自然胶片颗粒感（film grain），背景层次丰富，

有真实氛围感，

眼部具备清晰的眼神光（catchlight），与自然对焦效果，

面部带有微妙情绪表情，眼神灵动不呆滞；

肢体具备真实重量感，动态动作体现自然的力度传导，

衣物衣角随身体动作随性自然摆动，姿态松弛舒展；

皮肤呈现原生真实质感，可见自然毛孔、微细血管，

肤色自然红润，保留真实微小皱纹。
```

## 负面提示词（排除 AI 感通病）

```
干净无层次的背景，眼神空洞无神，面部表情僵硬，

肢体僵硬漂浮，动作不符合物理逻辑，塑料感皮肤，

陶瓷般光滑肌肤，过度磨皮，无瑕假脸，AI失真感，

过度完美的不真实质感
```

## 使用方式

- 直接把「完整提示词」作为风格/质量锚点拼接到任何角色图提示词前面。
- 反向清单放进 negative prompt 区块（Midjourney 用 `--no`、SD 用 Negative LoRA、即梦用「不希望出现」字段）。

## 触发词

- 真实感、去AI感、写实、电影级、cinematic realism、anti-AI、皮肤质感、photo real

## 与其他 reference 的关系

- 皮肤细节补充 → `references/skin-texture-banks.md`
- 光影层次补充 → `references/portrait-lighting-banks.md`
- 表情生动性 → `references/facial-expression-banks.md`
- 通用质量门控 → `references/quality-control.md`
