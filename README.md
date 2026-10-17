# 霓光連斬 NEON SLASH

霓虹風格的俯視角動作小遊戲：走位、瞄準，用衝刺斬擊敵人，撐過一波波攻勢、刷新最高分。

**▶ 線上遊玩：<https://wenbin2005.github.io/neon-slash/>**

支援電腦（鍵盤滑鼠、手把）與手機瀏覽器（觸控）。第一次進入會先開新手教學。

## 操作

| 動作 | 鍵盤滑鼠 | 手把 | 手機觸控 |
|---|---|---|---|
| 走位 | WASD／方向鍵 | 左搖桿 | 左半邊拖動 |
| 瞄準 | 滑鼠 | 右搖桿 | 左半邊拖動 |
| 衝刺 | 滑鼠左鍵／Space | RT／RB | 右半邊點擊 |
| 開始 | 點擊／Enter | A | 點擊 |
| 重開 | R | Start | 點擊 |
| 回標題 | Esc | B | 點右上「返回」 |

鍵盤另有：M 靜音、T 減少震動、H（標題畫面）新手教學。

## 系統需求

- 支援 WebGL 2 與 WebAssembly 的瀏覽器，並且要啟用 JavaScript。
- 手機建議橫向遊玩：直向開啟時會先出現「請把手機轉成橫向」的提示，也可以選擇直向繼續。
- 第一次載入要下載約 12 MB 的建置檔；網路慢或裝置較舊時要等久一點，載入畫面會顯示進度。

## 這個 repo 放什麼

- Unity WebGL 的建置檔：`index.html`、`Build/`、`TemplateData/`。沒有原始碼。
- 其他：本說明、`licenses/`（字型授權）、`.nojekyll`（讓 GitHub Pages 原樣提供檔案）、`.gitattributes`（所有檔案不做換行轉換，維持和建置相同的位元組）。
- 建置有網域鎖：只在官方網址所在的主機 `wenbin2005.github.io` 執行（只比對主機，不比對路徑）。放到其他網址（包括自己架的伺服器）或被其他網站用 iframe 嵌入時，會停在「只能在官方網址遊玩」的畫面；直接雙擊 `index.html` 開啟，瀏覽器不會載入遊戲。網域鎖在瀏覽器端檢查，用來防止直接轉載，不是完整的防護。
- 建置：Unity 6000.6.3f1，2026-10-07。

## 已知限制

- 網域鎖在瀏覽器端檢查，只能提高轉載的門檻，不是完整的防護；它限制的是「在哪裡執行」，不限制誰能玩。
- 遊戲要透過網址開啟：直接雙擊 `index.html`（`file://`）不會載入。

## 授權

- 遊戲內容 © 2026 wenbin2005，保留所有權利。未經同意請勿轉載、重新發布或另外架設。
- 建置內含兩套字型，都以 SIL Open Font License 1.1 授權：介面字型 NeonSlash UI TC（Noto Sans TC 的子集修改版），以及 Unity 內建的 Liberation Sans。說明見 [`licenses/FONT-LICENSE.txt`](licenses/FONT-LICENSE.txt)，授權全文見 [`licenses/OFL.txt`](licenses/OFL.txt)。
