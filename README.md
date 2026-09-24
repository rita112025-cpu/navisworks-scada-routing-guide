# Navisworks SCADA 線槽配置判斷指南 | SCADA Cable Tray Routing Guide

> 只保留已查證內容，未查證項目明確標示 ✅ 官方來源可追溯

[[Navisworks](https://img.shields.io/badge/Navisworks-2025%2B-FFC72C?style=flat-square)](https://help.autodesk.com/cloudhelp/2025/ENU/Navisworks/)
[[Language](https://img.shields.io/badge/Language-繁中%20%2F%20简中%20%2F%20EN-blue?style=flat-square)]()
[[License](https://img.shields.io/badge/License-MIT-green?style=flat-square)]()

一個給現場 BIM / MEP 工程師的 **Navisworks 判斷 SCADA 線槽能否配置** 的實戰操作手冊。從剖面切法、俯視/側視判斷、淨空量測、到最後的 Clash 檢查，全部步驟化，並附上**官方中文版按鈕中英對照表**。

An open, verified field guide for BIM/MEP engineers to check SCADA cable tray routability in Navisworks, with official Chinese UI translations.

---

## ✨ 特色 Features

- **已查證優先**：每個按鈕位置標註 ✅官方 / 🔸第三方 / ，不瞎寫
- **中文版對照**：英文介面 → 简体中文 → 繁體中文，官方手冊標準譯名
  - 例如：`Viewpoint > Sectioning > Enable Sectioning` → `视点 > 剖分 > 启用剖分` / `視點 > 剖切 > 啟用剖切`
- **大字閱讀版 + 暗色模式**：工地/機房也看得清楚，支援亮/暗主題切換
- **美化網頁版**：可直接當作內部教育訓練教材，一鍵開啟即用
- **包含完整流程圖**：`Box 框樓層 → 調高度 → 俯視看路徑 → 控制顯示 → 側視看高度 → Measure → 存 Viewpoint → Clash`

---

## 📂 建議的 Repo 名稱

推薦 3 個，依你的偏好選一個：

1.  **`navisworks-scada-routing-guide`** ⭐ 最推薦，SEO 最好
2.  `bim-navisworks-scada-tray-guide`
3.  `navisworks-tw-scada-cheatsheet`

GitHub 簡介 (Description) 可以直接貼這段：

> Navisworks 現場判斷 SCADA 線槽能否配置的實戰指南，含中英對照按鈕位置、剖分/框選技巧、淨空量測與 Clash 檢查，附美化網頁版教材。

Topics / Tags 建議加上：

`navisworks` `bim` `scada` `mep` `cable-tray` `clash-detection` `autodesk` `bim-guide` `繁體中文`

---

## 🚀 快速開始

### 線上看網頁版
直接打開 `docs/index.html`，就是最新版的大字+暗色模式版。

### 現場操作精簡版 (30秒版)

1.  **開剖面**：`視點 > 剖切 > 啟用剖切` → 模式選 `方塊(Box)`，框出目標樓層
2.  **調高度**：上緣蓋到上層樓板下緣，下緣蓋到天花板，寧可先厚一點
3.  **俯視看路徑**：ViewCube 點 TOP + `視點 > 相機 > 正投影`
4.  **控制顯示**：建築/樓板設透明，樑、風管、消防管、既有線槽一定要保留
5.  **側視看高度**：前視/右視確認是走樑下還是風管下
6.  **量淨空**：`審閱 > 測量 > 點對點 / 最短距離`
7.  **存起來**：`視點 > 儲存、載入與播放 > 儲存視點` 命名如 `2F_SCADA_平面`

---

## 📖 中英對照速查表 (節錄)

| 功能 | 繁中 (TW) | 简中 (CN) | 英文 |
|---|---|---|---|
| 開啟剖面 | 視點 > 剖切 > 啟用剖切 | 视点 > 剖分 > 启用剖分 | Viewpoint > Sectioning > Enable Sectioning |
| 框選模式 | 剖切工具 > 模式 > 方塊 | 剖分工具 > 模式 > 框 | Sectioning Tools > Mode > Box |
| 移動/旋轉/縮放 | 轉換 > 移動 / 旋轉 / 縮放 | 变换 > 移动 / 旋转 / 缩放 | Transform > Move / Rotate / Scale |
| 正投影 | 視點 > 相機 > 正投影 | 视点 > 相机 > 正交 | Viewpoint > Camera > Orthographic |
| 隱藏 | 常用 > 可見性 > 隱藏 | 常用 > 可见性 > 隐藏 | Home > Visibility > Hide |
| 透明度 | 項目工具 > 外觀 > 透明度 | 项目工具 > 外观 > 透明度 | Item Tools > Appearance > Transparency |
| 量測 | 審閱 > 測量 > 點對點 | 审阅 > 测量 > 点到点 | Review > Measure > Point to Point |
| 碰撞檢查 | 常用 > 工具 > 碰撞偵測 | 常用 > 工具 > 碰撞检查 | Home > Tools > Clash Detective |

> 完整對照表請看網頁版頂部可搜尋表格

---

## 📁 建議的檔案結構

```
navisworks-scada-routing-guide/
├─ README.md              # 你現在看的這個
├─ README_EN.md           # 英文版 (可選)
├─ docs/
│  ├─ index.html          # 美化網頁版 (大字+暗色模式)
│  └─ assets/             # 圖片、圖標 (可選)
├─ src/
│  ├─ 01_整體流程.md       # 原始流程 markdown
│  └─ 02_按鈕位置.md       # 原始按鈕位置 markdown
├─ LICENSE
└─ .gitignore
```

---

## 🔍 來源 Sources

- [Navisworks Help | Sectioning](https://help.autodesk.com/cloudhelp/2025/ENU/Navisworks/files/GUID-FEEA00D6-CEFA-47B5-8E6D-CFDF4E33428B.htm)
- [Measure Tools](https://help.autodesk.com/cloudhelp/2023/ENU/Navisworks/files/GUID-7F093364-2A34-41F9-BFD2-5B844DA1FDC0.htm)
- [Autodesk Navisworks Simulate 2012 用户手册 (官方中文)](http://images.autodesk.com/adsk/files/autodesk_navisworks_simulate_2012_user_guide_chs.pdf)
- [Create and Use Sets](https://help.autodesk.com/cloudhelp/2023/ENU/Navisworks/files/GUID-8FD0DD39-EC51-4C2F-BD60-6F84A3540E52.htm)
- [Clash Detective Select Tab](https://help.autodesk.com/cloudhelp/2026/ENU/Navisworks-Clash-Detective/files/GUID-F72265A1-A934-4533-9377-87DC3DB1519A.htm)

> 標註的項目代表本次未找到官方文件，已在文中明確標示，避免誤導。

---

## 🤝 貢獻

歡迎 PR！尤其是：
- 補上中文版 2025/2026 的新截圖
- 補上你們公司實際的 SCADA 線槽命名規則
- 翻譯成其他語言

---

## 📄 License

MIT License - 可自由用於公司內訓、專案文件。

---

## 作者

Chung Yu Cheng | 台北 / 武漢

> Made for field engineers who actually have to climb and measure.