# NL2SQL Agent 2.0 · 零基礎圖解導覽

用中文問資料庫，答案附上 SQL 與圖表。這個頁面把 NL2SQL Agent 2.0 的「寫 SQL 之前」與「執行 SQL 之前」各做了什麼把關，拆成可點、可試玩的圖解。

- 互動頁（GitHub Pages）：https://jamic710808.github.io/nl2sql-agent-intro/
- 互動頁（Vercel）：https://nl2sql-agent-explainer.vercel.app

## 頁面內容
- 68 秒旁白介紹影片（Gemini 3.8 Flash TTS · Kore），可點章節跳轉
- 可點的架構圖：比喻名／技術名切換，附程式位置
- 一個問題的旅程（5 步）與四道關卡（澄清先行、語意注入、JOIN 路徑、語法樹守衛）
- 「澄清判定」試玩：規則取自 `agent.py` 的 5 組關鍵字
- 「SQL 守衛」案例：7 個 SQL 的放行／擋下判定
- 後台五個工作台的真實截圖與熱點說明
- 「已確認事實」與「觀察／待確認」兩欄

## 如實說明
- 畫面為 2026-09-19 本機實拍與重製介面，資料表為範例與測試上傳資料。
- 「SQL 守衛」案例依 `sql_guard.py` 逐行推演，**未實際執行**。
- 「怎麼跑起來」依 README 與 Dockerfile 整理，**未實際啟動服務**。
- 旁白的發音與音量未經人耳確認。
- 2.0 功能在 `backend-overhaul` 分支，尚未併入 `main`。

本倉庫為輕量版：`index.html` 約 100 KB，圖片與影片是 `assets-2026-10-12-nl2sql/` 內的獨立檔案（影片串流播放，載入較快）。Vercel 版是單檔自包含（圖片與影片內嵌，約 11.7 MB），可直接另存使用。
