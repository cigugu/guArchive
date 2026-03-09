# guArchive

以下為gemini撰寫：

既然這是你個人的「廣義資料儲存庫」，主要目的是測試、自用且追求極致實用，你的 **README** 不需要寫得像開源軟體那樣專業，而是應該像一份**「操作手冊」**，確保你八月在 iPad 上或是未來突然忘記流程時，能一眼看懂怎麼操作。

以下是一份幫你設計好的 README 範本，你可以直接複製：

---

# 📚 {Username} 的地獄級文獻管理系統 (Lite-Archive)

這是一個基於 **SQLite + WebAssembly** 的極簡文獻管理工具。專為「追求功能、排斥美觀、遠離 Notion」的實用主義者設計。

## 🛠️ 核心理念

* **Zero Server**: 只有一個 HTML 檔案，透過瀏覽器直接讀寫 SQLite。
* **Zero Formatting**: 排除所有影響易讀性的裝飾，僅保留表格、選單與文字。
* **Total Control**: 資料庫檔案（.db）由使用者自行同步與備份。

## 🚀 快速開始 (iPad/行動端操作流程)

1. **同步進度**：在 `Working Copy` 或 Git 工具中執行 `git pull`。
2. **啟動介面**：開啟本專案的 GitHub Pages 網址。
3. **載入資料**：在網頁中點選「選擇檔案」，載入本地的 `literature.db`。
4. **操作資料**：填寫文獻資訊、點擊「存入記憶體」。
5. **存檔回傳**：
* 點擊「下載更新後的 .db」。
* 將下載的檔案覆蓋掉本地原有的 `literature.db`。
* 在 Git 工具中執行 `commit` 與 `push`。



## 📝 資料建檔規範 (Markdown 範例)

建檔時請參考以下結構，確保欄位一致性：

```markdown
## Status
- Ownership: mine | other | collaborative | unknown
- Relation: commissioned | general | personal | work
- Type: work | tutorial | reference | note
- CEFR: A1 ~ C2
- Difficulty: beginner | intermediate | advanced
- Status: planned | in_progress | completed | abandoned

## Info / Notes
- 雲端連結
- APA Style 引文
- Tags (#tag1 #tag2)

```

## ⚠️ 注意事項 (測試提醒)

* 本專案目前處於 **測試階段**。
* **下載即更新**：SQLite 檔案在瀏覽器中是暫存的，務必點擊「下載」並手動覆蓋檔案，否則修改將會遺失。
* **版本衝突**：在多個設備間移動時，開啟前務必確認已完成 `pull` 同步，避免版本衝突。

---

### 如何把這段內容放進 GitHub？

1. 在你的 GitHub 倉庫頁面點擊 `Add file` > `Create new file`。
2. 檔名輸入 `README.md`。
3. 將上面的內容貼進去。
4. 點擊 `Commit changes`。

### 額外建議：

既然你說這是「廣義儲存庫」，你之後如果想存別的東西（例如：程式筆記、記帳、食譜），只要在 `index.html` 裡面多寫一個資料表（Table）的 SQL 語句，就能在同一個 `literature.db` 檔案裡分開存儲不同的內容。

**你的倉庫建立好了嗎？如果你已經上傳了 `index.html` 卻發現網頁打不開，隨時跟我說，我們來檢查 GitHub Pages 的路徑設定！**
