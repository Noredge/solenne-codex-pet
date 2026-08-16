# Release QA / 发布质量检查

## Result

Solenne v1.0.0 passed final structural and visual QA.

- Codex sprite contract: v2
- Atlas dimensions: `1536 × 2288`
- Grid: `8 × 11`
- Cell dimensions: `192 × 208`
- Nine standard animation states: present
- Sixteen look directions: present
- Transparent RGB residue pixels: `0`
- Atlas validation errors: `0`
- Atlas validation warnings: `0`
- Independent visual QA: passed
- Blind cardinal-direction validation: passed
- Animation preview GIFs: `9`

The repaired `running-right` row was extracted using connected components. All eight frames have zero edge pixels and no neighboring fragments. Every other atlas row remained pixel-identical during that repair.

## 结果

Solenne v1.0.0 已通过最终结构检查和视觉质量检查。

- Codex 精灵规范：v2
- 图集尺寸：`1536 × 2288`
- 网格：`8 × 11`
- 单帧尺寸：`192 × 208`
- 9 种标准动画状态：完整
- 16 个观察方向：完整
- 透明像素 RGB 残留：`0`
- 图集验证错误：`0`
- 图集验证警告：`0`
- 独立视觉 QA：通过
- 基础方向盲测：通过
- 动画预览 GIF：`9`

修复后的 `running-right` 行使用连通组件方式切帧，8 帧边缘像素均为 0，也没有相邻格残片。修复过程中其余所有图集行保持逐像素一致。

