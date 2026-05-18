# codex-lazy-packs — AGENTS.md

## 專案入口

專案名稱：codex-lazy-packs
專案用途：整理並維護 OpenAI Codex 版懶人包，提供老師依照 Markdown 文件完成環境建置、MCP 連線、資料庫、Obsidian、GitHub 與專案工作流程設定。
主要工作目錄：D:\2026 database\codex-lazy-packs
GitHub repo：https://github.com/z334096-glitch/codex-lazy-packs.git
上游 repo：https://github.com/mathruffian-dot/codex-lazy-packs.git
預設 branch：master

## Obsidian 對應筆記

Obsidian vault：D:\2026 CODEX
專案駕駛艙：codex-lazy-packs/專案工作流程.md
收工時優先更新：同上

> 注意：專案駕駛艙是 Obsidian vault 裡的一篇筆記，不是工作資料夾裡的 Markdown 檔。

## 工作桌 + 三個家

- 工作桌：D:\2026 database\codex-lazy-packs
- GitHub：https://github.com/z334096-glitch/codex-lazy-packs.git
- Obsidian：D:\2026 CODEX + codex-lazy-packs/專案工作流程.md
- Firebase：teacherstudy-109ef-d92e1

## 同步規則

開工時：
- 使用 `startup-sync` 流程
- 讀本檔
- 讀 Obsidian 駕駛艙
- 檢查 Git 狀態
- 不自動 pull / commit / push

收工時：
- 使用 `shutdown-sync` 流程
- 更新 Obsidian 駕駛艙
- 如規則、路徑、專案邊界改變才更新本檔
- 需要時 commit + push GitHub

新專案初始化時：
- 使用 `project-init-sync` 流程
- 既有專案先盤點已存在與缺少項目，只補缺口
- 不覆蓋既有 README、.gitignore、AGENTS、Firebase 設定或 Git 歷史

## 主要檔案

入口檔：
- README.md：懶人包總覽與使用入口
- 00-環境建置.md 到 09-用chezmoi同步Codex設定.md：各章懶人包

設定檔：
- .gitignore：排除本機設定、敏感資訊與建置輸出
- AGENTS.md：Codex 專案規則
- CLAUDE.md：Claude Code 平行版提示

部署位置：
- GitHub repo：z334096-glitch/codex-lazy-packs
- 上游參考：mathruffian-dot/codex-lazy-packs

## 不要做

- 不要把每日進度寫進 AGENTS.md
- 不要自動納入無關 Git 變更
- 不要把 API key、token、密碼寫進 repo
- 不要把 `.codex/`、`.claude/` 或本機認證資料 commit
- 不要儲存學生姓名；正式資料只用座號與班級代號
- 不要把 Claude Code 版內容直接複製成 Codex 版；MCP 指令、設定檔格式、Skill 機制要轉成 Codex 寫法
