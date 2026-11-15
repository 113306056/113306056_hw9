# 區塊鏈機制解剖室 Crypto Mechanism Lab

把加密貨幣與 DeFi 的機制拆成固定格式：**流程圖、角色、風險、常見誤解、延伸閱讀**。


## 目前的標本

| 頁面 | 類別 | 難度 |
|---|---|---|
| 資金費率 Funding Rate | 衍生品 | 入門 |
| 套利 Arbitrage | 交易策略 | 入門 |
| 最大可提取價值 MEV | 區塊鏈基礎設施 | 進階 |
| Morpho 隔離式借貸市場 | 借貸 | 進階 |

## 專案結構

```
├── AGENTS.md          AI 的規則書（先讀這份）
├── index.html         首頁
├── assets/style.css   全站樣式
├── mechanisms/        每個機制一頁
└── templates/         新增頁面的模板
```

## 本機預覽

純靜態網站，不需安裝任何東西。直接用瀏覽器開啟 `index.html`，或在專案資料夾執行：

```
python3 -m http.server 8000
```

然後打開 http://localhost:8000。

## 部署到 GitHub Pages

1. 在 GitHub 建立新的公開 repository（例如 `crypto-mechanism-lab`）。
2. 把本資料夾的所有檔案上傳（包含 `.nojekyll`）。
3. 進入 repository 的 Settings，選 Pages。
4. Source 選 `Deploy from a branch`，Branch 選 `main`，資料夾選 `/ (root)`，儲存。
5. 等一到兩分鐘，網址會是 `https://<你的帳號>.github.io/<repository 名稱>/`。

## 如何新增一頁

對 AI 說：

> 請先讀 AGENTS.md，然後新增「閃電貸」頁，類別放「交易策略」，難度進階。

AI 會依 `AGENTS.md` 第 7 節流程：複製模板、填五個區塊、更新首頁與進度表，並回報哪些地方標了「待查證」。

## 免責聲明

本專案不構成任何投資建議。
