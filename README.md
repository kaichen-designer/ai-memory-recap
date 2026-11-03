# AI 回憶錄（原型）

把你和 AI 一起工作的紀錄，變成一張只屬於你的回顧卡。

## 怎麼用

1. 用 Chrome 或 Edge 開啟頁面。
2. 把 AI 的紀錄放進來，可以分次加入多個工具：
   - Claude Code：`%USERPROFILE%\.claude\projects` 資料夾（Mac、Linux 是 `~/.claude/projects`）
   - ChatGPT、Claude.ai：在設定裡匯出資料，解壓縮後選 `conversations.json`
3. 按「產生我的回憶錄」。

## 隱私

- 所有計算都在你的瀏覽器裡完成，頁面設定為禁止任何網路連線。
- 只讀取 `projects` 底下的 `.jsonl` 與 `conversations.json`，其他檔案一律忽略。
- 整個頁面就是 `index.html` 一個檔案，歡迎自己檢查。
- 投影或分享畫面前，按「遮蔽原話」（快捷鍵 P）可以把引用的話模糊掉。

## 目前的限制

- ChatGPT 與 Claude.ai 的解析只用模擬資料測過，尚未用真實匯出檔驗證。
- Gemini、Codex 尚未支援。
- Firefox、Safari 未測試。
