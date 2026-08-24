# 經典調酒吧 (Grade B Classic 90 Cocktails Guide) 🍹

一個基於純前端技術（HTML5 + Tailwind CSS CDN + Vue 3 CDN + Lucide Icons）打造的「**乙級經典 90 款調酒指南**」與「**我的吧台**」庫存匹配系統。

專為飲料調製技能檢定（乙級證照）學習者、調酒愛好者與居家調酒師設計，提供極致流暢、深色暗黑金屬質感 (Dark Slate) 與 8-Bit 像素風格的互動體驗。

---

## 🌟 核心功能特色

- 🍸 **完整 90 款經典調酒資料庫**
  - 包含中文/英文名稱、六大基酒、調製手法 (Shake / Stir / Build / Blend / Layer)、專用杯型、酒精濃度 (ABV %)、酒感星級 (1-5★)、預估熱量 (kcal) 及風味標籤。
  - 收錄 **乙級考照規範裝飾物** 與 **居家替代建議 (Home Hack)**。
  - **CORS 零阻礙 Fallback 機制**：內建數據備援機制，即使直接雙擊 `file://index.html` 開啟或上傳至 GitHub Pages 皆能 100% 正常運行。

- 🧊 **「我的吧台」庫存匹配系統 (My Bar)**
  - 四大材料分區：**六大基酒**、**香甜酒/利口酒**、**副材料/軟性飲料**、**生鮮裝飾/其他**。
  - 支援分類折疊/收合與一鍵勾選。
  - 即時計算可調調酒：
    - **【100% 即可調製 (Ready to Drink)】**
    - **【缺 1 種材料 (Missing 1)】**：卡片高亮缺料，點擊彈窗即刻提供 Home Hack 替代指南。
  - 勾選狀態自動備份於 `localStorage`。

- 🎲 **「今晚喝什麼？」隨機轉盤 / 雪克杯動畫**
  - 觸發 1.5 秒 3D 雪克杯 Shake 抖動 CSS 動畫。
  - 內建 **Web Audio API** 音樂合成器，發出模擬冰塊碰撞金屬雪克杯的真實音效。
  - 隨機抽取調酒並跳出推薦彈窗 Modal。

- 🔍 **全域搜尋與多維過濾**
  - 支援中英文名稱、材料、風味關鍵字模糊搜尋。
  - 支援「六大基酒」、「酒精濃度分級 (無酒精 / <15% / 15-25% / >25%)」、「調製手法」與「排序」過濾。

- 📏 **容量單位一鍵切換**
  - 支援公制毫升 `ml` 與英制盎司 `oz` 單位無縫轉換。

---

## 🚀 部署至 GitHub Pages 教學

若您想將此網站發布在 GitHub 上供其他人線上瀏覽，請依照以下簡單步驟操作：

### 步驟一：上傳程式碼至 GitHub

1. 在 [GitHub 官網](https://github.com/) 點擊右上角 `+` -> **New repository**。
2. 設定 Repository Name（例如：`cocktails-bar`），權限選擇 **Public**（公開），然後點擊 **Create repository**。
3. 在本機專案目錄（終端機/PowerShell）執行以下指令：

```bash
# 綁定您的 GitHub 遠端倉庫（請替換 USERNAME 為您的 GitHub 帳號）
git remote add origin https://github.com/USERNAME/cocktails-bar.git

# 切換預設分頁名稱為 main
git branch -M main

# 推送程式碼至 GitHub
git push -u origin main
```

---

### 步驟二：開啟 GitHub Pages 免費網址

1. 進入您在 GitHub 上的 repository 頁面。
2. 點選上方頁籤 **Settings**（設定）。
3. 在左側選單點選 **Pages**。
4. 在 **Build and deployment** 下方的 **Source** 選擇 **Deploy from a branch**。
5. Branch 選擇 **`main`** 並且目錄選擇 **`/(root)`**，點擊 **Save**。
6. 等待 1~2 分鐘，頁面上方即會出現您的專屬線上網址：
   `https://USERNAME.github.io/cocktails-bar/` 🎉

---

## 🛠️ 技術棧

- **HTML5** & **Vanilla JavaScript** (ES6+)
- **Tailwind CSS CDN** (Dark Slate Mode + Custom Pixel Shadows & Animations)
- **Vue 3 CDN** (Composition API / Reactive Engine)
- **Lucide Icons** (SVG Icon Kit)
- **Web Audio API** (Procedural Audio Synthesizer)
- **Google Fonts** (Noto Sans TC + DotGothic16 Pixel Font)

---

## 📄 授權條款

License: MIT License. 歡迎學習交流與改編！
