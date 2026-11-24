---
title: "系統架構與資料流程"
source_file: "呆萌居家AI管家專案/docs/architecture.md"
document_type: "project_knowledge"
ingestion: "完整 Markdown 原文匯入，附摘要與檢索標籤"
language: "zh-TW"
---

# 系統架構與資料流程

- **來源檔案：** `呆萌居家AI管家專案/docs/architecture.md`
- **匯入方式：** 保留原始 Markdown 全文，並附上摘要與檢索標籤。

## 知識摘要

整理使用者輸入、Agent、Planner、安全檢查、設備操作與 Writer 回覆之間的資料流程。

## 檢索標籤

`系統架構`, `資料流程`, `Planner`, `Writer`, `IoT`

## 原始資料（完整匯入）

```markdown
# 系統架構與資料流程

'''text
使用者（文字／語音）
        ↓
對話介面（Web／手機）
        ↓
AI Agent：理解意圖
        ↓
Planner：拆解任務、安排步驟
        ↓
安全與權限檢查
        ├── 查詢：感測器／設備狀態／用電資料
        └── 控制：使用者確認 → IoT 控制介面 → 智慧家電
        ↓
檢查工具或設備回傳結果
        ↓
Writer：整理親切清楚的回覆
        ↓
使用者收到結果
'''

## 範例：使用者說「家裡好熱！」
1. 理解使用者可能需要溫度資訊或冷氣協助。
2. Planner 安排查詢室內溫度及冷氣狀態。
3. 檢查感測器資料是否存在、是否過期。
4. 提出調整建議；控制前取得使用者確認。
5. 經授權後呼叫設備介面。
6. 讀取設備回傳狀態。
7. Writer 如實回報結果。

## 技術方向
- 前端：HTML、CSS、JavaScript。
- 後端：Python（可評估 Flask 或 FastAPI）。
- AI：大型語言模型 API。
- IoT：Wi-Fi、MQTT 或設備官方 API（依設備支援情況）。
- 感測器：溫度、濕度、智慧電表／智慧插座。

## 資料狀態
- `measured`：實際量測。
- `estimated`：系統估算。
- `simulated`：展示用模擬資料。
- `unavailable`：目前無法取得。
```
