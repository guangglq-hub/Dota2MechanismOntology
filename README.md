# Dota2 Mechanism Ontology Dist

## 中文说明

这个仓库用于存放 Dota 2 机制本体项目编译后的 `dist/` 最终产物，面向运行时检索、RAG 召回和应用侧消费，不承载原始标注与规则编辑过程。

### 仓库内容

- `dist/hero_profiles.json` - 英雄派生画像
- `dist/item_profiles.json` - 物品派生画像
- `dist/skills.json` - 技能层结构化数据
- `dist/relation_edges.json` - 跨英雄/技能/物品的关系边
- `dist/indexes.json` - 画像、特征、关系等索引
- `dist/retrieval_blocks.json` - 面向 RAG 的检索块
- `dist/README.md` - 检索块类型与分布说明

### 使用方式

这些文件是机制知识库流水线产出的运行时结果。

1. 在上游本体项目中维护原始知识、标注和规则。
2. 重新生成最新的 `dist/` 产物。
3. 将更新后的 `dist/` 同步到本仓库。

应用侧应优先读取 `dist/` 中的结构化结果，而不是直接读取源 Markdown 或规则文件。

## English

This repository stores the compiled `dist/` artifacts for the Dota 2 mechanism ontology project. It is intended for runtime retrieval, RAG consumption, and application-facing integration, rather than source authoring.

### Contents

- `dist/hero_profiles.json` - derived hero profiles
- `dist/item_profiles.json` - derived item profiles
- `dist/skills.json` - structured skill-layer data
- `dist/relation_edges.json` - relation edges across heroes, skills, and items
- `dist/indexes.json` - indexes for profiles, traits, and relations
- `dist/retrieval_blocks.json` - RAG-ready retrieval blocks
- `dist/README.md` - retrieval block type and distribution summary

### Intended Use

These files are the runtime-facing outputs of the ontology pipeline.

1. Maintain source knowledge, annotations, and rules in the upstream ontology project.
2. Rebuild the latest `dist/` artifacts there.
3. Sync the refreshed `dist/` directory into this repository.

Application code should read from `dist/` instead of directly consuming source Markdown or rule files.
