---
title: "專案總覽"
source_file: "呆萌居家AI管家專案/README.md"
document_type: "project_knowledge"
ingestion: "完整 Markdown 原文匯入，附摘要與檢索標籤"
language: "zh-TW"
---

# 專案總覽

- **來源檔案：** `呆萌居家AI管家專案/README.md`
- **匯入方式：** 保留原始 Markdown 全文，並附上摘要與檢索標籤。

## 知識摘要

說明專案定位、資料夾結構、開始方式，以及範本目前的實作狀態。

## 檢索標籤

`專案概覽`, `目錄結構`, `啟動`, `模擬資料`

## 原始資料（完整匯入）

```markdown
# 呆萌居家 AI 管家

以 Planning Agent 為核心的智慧家庭助理專案。使用者可透過自然語言查詢家庭狀態、取得生活建議，並在授權後操作相容的智慧家電。

## 資料夾結構
'''text
呆萌居家AI管家專案/
├── AGENTS.md
├── README.md
├── docs/
│   ├── project_spec.md
│   └── architecture.md
├── prompts/
│   ├── PLANNER_PROMPT.md
│   └── WRITER_PROMPT.md
├── src/
│   └── index.html
├── assets/
└── tests/
    └── test_scenarios.md
'''

## 開始方式
1. 使用 VS Code 開啟本資料夾。
2. 閱讀 `AGENTS.md`，遵循角色、安全及開發規範。
3. 從 `src/index.html` 開始開發前端。
4. 初期使用模擬資料時，必須明確標示「模擬」。
5. 後續再整合 AI API、感測器與智慧家電。

## 目前狀態
這是專案文件與程式架構起始範本。尚未連接真實 AI 模型或智慧家電。
```
