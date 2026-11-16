# JSONL 字段
两个文件都只追加，不覆盖，一行一个 JSON 对象。
## pushed.jsonl
```json
{"date": "2026-11-16", "slot": "一线实践", "id": "20261116-1", "title": "……", "author": "……", "url": "https://……", "lang": "en", "in_circle": true, "verified": true, "month_question": "什么内容会爆？我在读者心里是谁？"}
```
- `slot`：一线实践 / 深度材料 / 一个人 / 一个反面观点 / 一个输出题 / 一本书 / 一个跨界输入 / 一次回顾
- `id`：日期加条目编号，用户回「3 有用」时据此定位
- `in_circle`：是否在用户兴趣圈内，用于统计每周 20% 圈外比例
- `verified`：链接和关键信息是否已实时核实
## feedback.jsonl
```json
{"date": "2026-11-16", "target_id": "20261116-3", "signal": "有用", "reason": "", "action": "多推一人商业写作者"}
```
- `signal`：有用 / 没用 / 太浅 / 换题 / 回顾
- `reason`：用户给的原因，「没用」时问一句后填
- `action`：你据此做了什么调整
