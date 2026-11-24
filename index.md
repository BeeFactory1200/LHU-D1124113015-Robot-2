---
title: "呆萌居家 AI 管家｜LLM Wiki"
version: "1.0"
language: "zh-TW"
ingested_documents: 7
---

# 呆萌居家 AI 管家｜LLM Wiki

本知識庫由上傳的 `呆萌居家AI管家專案範本.zip` 建立。

## Ingestion 結果

- **已 ingest：7 篇 Markdown 來源文件**
- **最低要求：5 篇 — 已達成**
- **輸出格式：** Markdown Wiki
- **匯入原則：** 每篇來源文件各自建立一個 Wiki 頁面，保留全文，並加入摘要、來源檔名與檢索標籤。

## Wiki 頁面索引

- [Agent 專案指引](pages/agent-project-guide.md) — 整理專案目標、Agent 工作流程、Planner/Writer 分工、安全隱私原則與開發規範。（來源：`呆萌居家AI管家專案/AGENTS.md`）
- [專案總覽](pages/project-overview.md) — 說明專案定位、資料夾結構、開始方式，以及範本目前的實作狀態。（來源：`呆萌居家AI管家專案/README.md`）
- [系統架構與資料流程](pages/system-architecture.md) — 整理使用者輸入、Agent、Planner、安全檢查、設備操作與 Writer 回覆之間的資料流程。（來源：`呆萌居家AI管家專案/docs/architecture.md`）
- [專案需求規格](pages/project-requirements.md) — 彙整專案動機、功能需求、非功能需求與開發階段。（來源：`呆萌居家AI管家專案/docs/project_spec.md`）
- [測試情境](pages/test-scenarios.md) — 整理專案測試案例及各情境預期的安全行為與回應。（來源：`呆萌居家AI管家專案/tests/test_scenarios.md`）
- [Writer 提示詞](pages/writer-prompt.md) — 記錄 Writer 如何將規劃整理成親切清楚的繁體中文回覆，並誠實呈現執行狀態。（來源：`呆萌居家AI管家專案/prompts/WRITER_PROMPT.md`）
- [Planner 提示詞](pages/planner-prompt.md) — 記錄 Planner 如何理解需求、拆解任務、安排步驟並考量設備狀態、安全與權限。（來源：`呆萌居家AI管家專案/prompts/PLANNER_PROMPT.md`）

## 核心概念速覽

- **任務流程：** 依來源文件所述，先理解需求，再規劃任務、檢查安全與權限、執行並回報。
- **Planner：** 負責需求分析、任務拆解、步驟安排與風險考量。
- **Writer：** 負責將規劃與執行狀態轉換為清楚、親切的繁體中文回覆。
- **安全原則：** 不應把模擬資料說成真實量測，也不應把預期結果說成已完成；設備操作須遵守來源文件所列的授權與確認要求。
- **狀態透明：** 對設備失聯、資料過期、工具失敗或無法取得的資訊，應清楚說明。

## 建議用來測試 Wiki 檢索的問題

1. Planner 和 Writer 的工作分別是什麼？
2. 使用者提出設備控制需求時，流程中有哪些安全檢查？
3. 專案包含哪些功能需求與開發階段？
4. 測試情境中有哪些設備操作案例？
5. 系統如何處理設備狀態無法取得或操作失敗的情況？

## 來源範圍說明

本 Wiki 內容以壓縮檔內實際找到的 Markdown 文件為依據；未加入外部資料。各頁面保留對應來源的原始文字，摘要與標籤僅作檢索輔助。
