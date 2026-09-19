# 本機材料（不進 git）

這個目錄被 [`.gitignore`](../.gitignore) 排除。公開 clone 不該看得到下面的檔。

| 檔案 | 為什麼不公開 |
| --- | --- |
| 2023 期末報告 `.docx` | 課堂報告；檔名與內文有學號、系級 |
| `ImpureDimwittedCottonmouth-max-1mb.gif` | 約 948 KB，程式從未 `getResource`；來源不明，不該進展示樹 |

`build/`、`dist/`、`nbproject/private/`、`nbproject/jfx-impl_backup*.xml` 仍在專案根目錄（NetBeans 再開會再生），只是同樣被忽略。

公開 README 的示範圖是從這份報告抽出的遊戲畫面，檔名已改成 `docs/assets/screenshot-*.png`，不含學號。需要對 2023 繳交原文時，在這台機器打開報告即可。請不要把這個目錄、學號或 GIF 推進公開分支。
