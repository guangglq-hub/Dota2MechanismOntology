# 检索块索引

总块数: 678

## 块类型分布
- effect_lookup: 64
- hero_item_need: 118
- hero_profile: 127
- item_hero_counter: 52
- item_profile: 190
- skill_upgrade: 127

## 块类型说明
- hero_profile: 英雄画像块，含特征/物品需求/克制/升级摘要
- item_profile: 物品画像块，含特征/效果/保护克制对象
- hero_item_need: 英雄物品依赖块，按英雄聚合所有依赖物品
- item_hero_counter: 物品英雄克制块，按物品聚合所有克制英雄
- skill_upgrade: 技能升级评估块，神杖/魔晶价值与详情
- effect_lookup: 效果时长速查块，按效果标签聚合所有技能/物品