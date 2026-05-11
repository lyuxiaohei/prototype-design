# prototype-design 文件结构对比（V3.0 → V3.2）

## V3.0 文件结构（13个文件）

```
prototype-design/
├── SKILL.md                              28,694B    主技能文件（路由+规范+组件+模板+资源）
├── reference.md                          16,767B    口述模式参考页面
│
├── rules/                                           模式识别与解析规则
│   ├── draft-parser.md                    8,240B    草案解析规则
│   ├── keyword-extractor.md               8,214B    口述关键词提取规则
│   ├── mode-detect.md                     4,582B    模式自动检测规则
│   └── page-type-inferencer.md            7,176B    页面类型推断规则
│
├── mappings/                                        草案→UI映射规则
│   ├── field-to-ui-element.md             9,353B    字段→UI元素映射
│   ├── navigation-to-flow.md              7,986B    页面导航→跳转映射
│   ├── state-to-interaction.md            8,918B    状态流转→交互映射
│   └── use-case-to-component.md           9,083B    功能用例→组件映射
│
├── validators/                                      输入输出验证
│   ├── input-validator.md                 8,857B    输入验证规则
│   └── output-validator.md                9,545B    输出HTML验证规则
│
└── reference/                                       参考资料
    └── draft-input-example.md            17,869B    草案输入示例
```

## V3.2 文件结构（21个文件）

```
prototype-design/
├── SKILL.md                              17,726B    主技能文件（路由+色彩+布局+索引）
├── README.md                              2,930B    仓库说明、文件结构、版本历史
├── reference.md                          16,767B    口述模式参考页面
├── 技能链协作指南.md                       3,629B    技能链协作说明
│
├── rules/                                           模式识别与解析规则
│   ├── draft-parser.md                    8,240B    草案解析规则
│   ├── keyword-extractor.md               8,214B    口述关键词提取规则
│   ├── mode-detect.md                     4,582B    模式自动检测规则
│   └── page-type-inferencer.md            7,176B    页面类型推断规则
│
├── mappings/                                        草案→UI映射规则
│   ├── field-to-ui-element.md             9,353B    字段→UI元素映射
│   ├── navigation-to-flow.md              7,986B    页面导航→跳转映射
│   ├── state-to-interaction.md            8,918B    状态流转→交互映射
│   └── use-case-to-component.md           9,083B    功能用例→组件映射
│
├── validators/                                      输入输出验证
│   ├── input-validator.md                 8,857B    输入验证规则
│   └── output-validator.md                9,545B    输出HTML验证规则
│
├── components/                           [新增]      组件CSS规范
│   ├── backend-components.md              1,334B    后台组件（按钮/网格/分页/分类树）
│   └── miniprogram-components.md          4,432B    小程序组件（框架/导航/Tab/卡片/弹窗等）
│
├── templates/                            [新增]      页面HTML模板
│   ├── backend-template.md                1,098B    后台页面骨架
│   └── miniprogram-template.md            1,163B    小程序页面骨架
│
└── reference/                                       参考资料
    ├── draft-input-example.md            17,869B    草案输入示例
    ├── resources.md                       1,764B    图标/图片素材网站推荐    [新增]
    └── svg-icons.md                       2,145B    小程序SVG图标代码库      [新增]
```

## 变化对比

| 指标 | V3.0 | V3.2 | 变化 |
|------|------|------|------|
| 文件总数 | 13 | 21 | +8 |
| 新增目录 | - | 2 | `components/`、`templates/` |
| SKILL.md 大小 | 28,694B | 17,726B | -38% |
| SKILL.md 行数 | 942行 | 460行 | -51% |
| 总内容量 | 149,786B | 149,786B | 不变（仅位置迁移） |

### V3.0 → V3.2 内容迁移明细

| 迁出内容 | V3.0 位置 | V3.2 位置 | 大小 |
|----------|-----------|-----------|------|
| 后台组件CSS | SKILL.md 1.4节 | `components/backend-components.md` | 1,334B |
| 后台HTML模板 | SKILL.md 1.5节 | `templates/backend-template.md` | 1,098B |
| 小程序组件CSS | SKILL.md 2.4节 | `components/miniprogram-components.md` | 4,432B |
| 小程序HTML模板 | SKILL.md 2.5节 | `templates/miniprogram-template.md` | 1,163B |
| 资源推荐网站 | SKILL.md 5.1+5.2节 | `reference/resources.md` | 1,764B |
| SVG图标代码 | SKILL.md 5.3节 | `reference/svg-icons.md` | 2,145B |
| 版本历史 | SKILL.md 六节 | `README.md` | - |

### 未变更文件（V3.0 → V3.2 内容完全一致）

- `rules/` 全部4个文件
- `mappings/` 全部4个文件
- `validators/` 全部2个文件
- `reference.md`
- `reference/draft-input-example.md`
