# ai-assistant-hub|AI 助理教學館

> 本專案受模型交接鐵律約束(`C:\Users\User\.claude\projects\C--Users-User\memory\future-model-ironlaw.md`):
> 過程可見、改動先問、對外動作先確認、異動紀錄必寫。

## 這是什麼

王少宇的「AI 助理教學館」——純靜態網站。兩個功能:

**部署(2026-07-10 起雙軌):**
- 主站:https://ai-assistant-hub-eosin.vercel.app/(Vercel,Web Analytics 溫度計已啟用;對外分享一律用這個)
- 備援:https://bruce97642.github.io/ai-assistant-hub/(GitHub Pages)
- `git push` 後兩邊自動部署;`.vercel/`、`.env*` 是機密,已 gitignore,絕不入 repo

1. **教學館**:三份完整指南(Claude 文書應用 / Gemini 解析 / ChatGPT×Codex 手冊),作為課程《AI 當你的助理》的課後資源與個人品牌門面
2. **測驗**:「你適合哪個 AI 助理?」六題測驗,結果頁導流到指南+FB(課程邀約入口)

## 檔案結構

- `index.html` — 首頁(三張指南卡+測驗 CTA+課程聯絡)
- `quiz.html` — 測驗(純前端計分,C/G/T 三型)
- `guides/claude.html` — Claude 指南(CHAT 生成的 artifact 原檔+加了頂欄)
- `guides/gemini.html` — Gemini 指南(由 MD 轉換,轉換腳本見異動紀錄)
- `guides/chatgpt.html` — ChatGPT 手冊(由 DOCX 轉換)
- `downloads/` — 原始檔下載(MD、DOCX)

## 慣例

- 教材原始檔的正本在 `G:\我的雲端硬碟\課程教材\三大AI助理入門課\原始教材\`,這裡的是發佈副本
- 內容標注「資訊基準:2026 年 7 月」,AI 工具改版後要更新
- 色系:Claude=#B3362B、Gemini=#3F6BB5、ChatGPT=#1F8A70、品牌金=#C99A2E
- 改版後在 `異動紀錄.md` 留一筆,commit + push 即自動部署(GitHub Pages)
