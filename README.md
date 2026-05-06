# 董立凱 2026 競選網站

**北區升級・立凱出擊**
彰化市市民代表 ・ 第三選區（北區）・ 台灣民眾黨提名

---

## 📁 檔案結構

```
dong-likai-2026/
├── index.html          # 主網站（單檔內含 CSS/JS）
└── images/             # 圖片資源
    ├── portrait.png    # 形象照（Hero）
    ├── leaders.jpg     # 與兩位主席合體（黨團合作）
    ├── traffic.jpg     # 民生地下道用路安全（實地會勘）
    ├── mazu.jpg        # 大甲媽祖繞境（在地信仰）
    ├── scooter.jpg     # 幫民眾牽摩托車（日常服務）
    └── team.jpg        # 與彰化民眾黨團隊
```

## 🚀 部署到 GitHub Pages

```bash
# 1. 建立新 repo（建議命名 dong-likai-2026 或 likai-2026）
# 2. 把整個資料夾推到 main 分支
git init
git add .
git commit -m "Initial campaign website"
git branch -M main
git remote add origin https://github.com/<your-username>/dong-likai-2026.git
git push -u origin main

# 3. 在 GitHub repo 的 Settings → Pages
#    - Source: Deploy from a branch
#    - Branch: main / root
#    - Save
# 4. 約 1–2 分鐘後即可從 https://<your-username>.github.io/dong-likai-2026/ 看到網站
```

## 🎨 設計重點

相較於先前的蘇智弦版本，這個網站做了以下升級：

1. **更專業的編輯式排版**：使用 Noto Serif TC + Fraunces 雙字型搭配，營造國際雜誌感
2. **更強烈的視覺層次**：從 Hero 形象照、跑馬燈、3 大支柱、政見列表到候選人 Dossier，每段節奏分明
3. **完整的政見呈現**：把 PDF 中的 SFS（Safety/Friendliness/Simplification）三大核心轉化為 6 條具體政見
4. **真實的服務足跡**：5 張照片說 5 個故事——黨團合作、實地會勘、在地信仰、日常服務、團隊
5. **轉換導向**：明顯的 CTA 按鈕、線上陳情表單、清晰的聯絡方式

## ⚙️ 客製化指南

### 修改聯絡資訊
搜尋 `0986-999-612` 與 `jack999612@gmail.com`，替換為實際使用的號碼/Email。

### 串接表單收件
目前表單為 demo（送出會跳 alert）。建議方案：
- **EmailJS**（免費版每月 200 封）：在 `<form>` 上加 `id="contact-form"`，用 EmailJS SDK 串接
- **Google Forms 嵌入**：直接把 `<form>` 替換為 Google Form iframe
- **Formspree**：把 `<form>` 改為 `<form action="https://formspree.io/f/xxxxx" method="POST">`

### 新增社群連結
搜尋 `社群連結籌備中`，替換為實際 FB / IG / YT / Threads 連結即可。

### 修改候選人資料
PDF 上的所有資料都已寫入 `<section class="profile">` 區塊，逐項對照修改即可。

## ⚠️ 法規提醒

- 網站底部已加入《公職人員選舉罷免法》與《政治獻金法》之網站設置聲明
- 正式上線前請：
  1. 與候選人本人逐項核對所有資料
  2. 確認所有照片皆已取得肖像權同意（特別是與第三人合照）
  3. 加入正式的「廣告刊登者」資訊（依法須揭露）

---

製作日期：2026/05
