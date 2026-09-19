# 貢獻指南

語言：[繁體中文](CONTRIBUTING.md) · [English](docs/CONTRIBUTING.en.md)

這是 2023 課程作業的封存 Showcase Repository。歡迎修文件、補「2026 年還能在 JDK 8 打開」的註記。請先當歷史文物看，再動手。

## 動工前

1. 讀根目錄 [`README.md`](README.md) 與 [`docs/README.md`](docs/README.md)。
2. 改規則或參數時，同步 [`docs/gameplay.md`](docs/gameplay.md) 與對應 Java。
3. 衝突時：**2023 繳交行為 > Showcase Repository 文件**。文件寫錯就改文件。遊戲邏輯只允許修「原檔明顯不能編譯／不能啟動」的缺陷，並寫進 [`docs/`](docs/)。

## 慣例

| 項目 | 約定 |
| --- | --- |
| 對外說明 | 繁中在 `README.md`；英文在 `docs/README.en.md`，兩邊一起改 |
| 日期 | `YYYY-MM-DD`，台北時間 |
| 變更紀錄 | `CHANGELOG.md` 的 `## [Unreleased]`（Keep a Changelog 2.0.0） |
| 換行 | LF（`.gitattributes`） |

## 請不要

- 提交 `local/`、`*.docx`、學號、`build/`、`dist/`、`nbproject/private/`、`jfx-impl_backup*`、未使用 GIF
- 在程式或文件裡硬寫本機絕對路徑、帳號、學號
- 把這份作業說成石門水庫的正式模擬或水利署產品
- 為了「比較現代」改寫成 Maven／JDK 21 卻聲稱這是 2023 原貌
- 替換手繪圖為官方水庫照片或台灣彩券／機關 logo（那些不屬於本專案）

不可逆的動作（force push、把報告打進歷史）請先問。

## 改完必做

1. Notable 變更寫進 `CHANGELOG.md` → `## [Unreleased]`
2. 動到 Hero／安裝／結構 → 繁中與英文 README 一起改
3. 若改了 `src/` 行為，在 [`docs/gameplay.md`](docs/gameplay.md) 註明與 2023 檔的偏離
