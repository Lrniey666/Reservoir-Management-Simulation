# 安裝與執行

語言：[繁體中文](installation.md) · 短版步驟見根目錄 [README.md](../README.md) 與 [README.en.md](README.en.md)

這是 **NetBeans 8 的 JavaFX 2／8 Ant 專案**。`javac.source` / `javac.target` 都是 `1.8`。主類別 `reservoir_management_simulation.Reservoir_Management_Simulation`。

## 還能開的組合

| 元件 | 2023 實況 | 2026 建議 |
| --- | --- | --- |
| JDK | Oracle JDK 8（JavaFX 在 `jre/lib`） | 仍用 JDK 8；Liberica **Full** 8 這類發行也帶 JavaFX |
| IDE | NetBeans 8.2rc | NetBeans 8.2 最省事。Apache NetBeans 新版對這份 `jfx-impl.xml` 不友善 |
| 建置 | Ant + `nbproject/jfx-impl.xml` | 用 IDE 的 Run，不要自己重寫 Maven／Gradle 還聲稱是原專案 |

`project.properties` 還列了 `javaws.jar`、`deploy.jar`、`plugin.jar`。那是 Java 8 桌上部署殘件，缺了也不影響在 IDE 裡 `start()`。

## 開專案

1. 安裝 JDK 8（確認 `java -version` 是 1.8）。
2. 安裝 NetBeans 8.2，JDK 指到同一套。
3. *File → Open Project* → 選含 `build.xml` 與 `nbproject/` 的目錄。
4. 屬性 → *Libraries / Platform* 選 JDK 8。
5. Run。標題列應為「水庫模擬器Beta」，畫布 1080×720。

第一次在新機器開，NetBeans 可能改寫 `nbproject/private/`。那個目錄已被 git 忽略，裡面會出現本機路徑（舊檔曾指向 Internet Explorer 與 `C:\Users\admin\...`）。

## 不要用的路

- **WebStart / 瀏覽器執行。** `nbproject/configs/Run_as_WebStart.properties` 與 `dist/*.jnlp` 還在磁碟上，但 Java 插件與 `java.com/js/dtjava.js` 已死。`dist/` 整棵忽略，不要把 jar 當發布物。
- **JDK 11+ 直接 `java`。** 模組系統裡沒有 `javafx.*`。若一定要在新 JDK 試，需另加 OpenJFX 模組路徑；那已超出「重現 2023 作業」的範圍，本倉不提供腳本。
- **只拷 `src/` 丟進別的範本。** FXML 用 `@晴天.png` 這種中文檔名相對路徑，資源必須與 `.class` 同目錄。

## 本機材料

[`local/README.md`](../local/README.md) 說明報告與 GIF 為什麼在那裡。公開 clone 看不到 `local/`。
