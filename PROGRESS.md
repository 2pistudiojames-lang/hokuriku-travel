# 北陸・中部 攝影旅遊指南 — 開發進度

## 專案資訊

- **本地路徑**：`/home/james/PROJECT_REBOOT/hokuriku-travel-site/`
- **GitHub Repo**：`2pistudiojames-lang/hokuriku-travel`
- **GitHub Pages**：https://2pistudiojames-lang.github.io/hokuriku-travel/
- **LAN 預覽**：http://192.168.1.115:4195/（systemd user service）
- **GitHub 帳號**：2pistudio.james@gmail.com / username: 2pistudiojames-lang

---

## 更新發佈流程

```bash
cd /home/james/PROJECT_REBOOT/hokuriku-travel-site
git add -A
git commit -m "描述這次改了什麼"
git push
```

---

## 開發里程碑

### 2026-05-02 v2 景點擴充 + Google Maps

**新增功能**
- 全部景點加入 Google Maps 📍 連結（點擊開啟定位）
- 富山 +1 景點：宇奈月溫泉 & 黑部峽谷鐵道
- 名古屋・岐阜 +4 景點：犬山城下町、長良川河畔、關ヶ原宿、飛驒古川
- 伊勢 +8 景點：二見興玉神社、托福橫丁街拍、伊雑宮、鳥羽水族館、橫山天空の郷、合歓の郷、猿田彥神社、河崎商人町

**景點統計**
- 金澤 14 景點 / 富山 15 景點 / 名古屋・岐阜 18 景點 / 伊勢 14 景點
- 共 **61** 個攝影景點，每個含 Google Maps 連結 + 拍攝建議
- 美食 32 家（各區 8 家，附 Google Maps）

**攝影筆記更新**
- 富山：加入宇奈月溫泉/黑部峽谷拍攝建議
- 名古屋：加入飛驒古川、關ヶ原、犬山城下町建議
- 伊勢：加入橫山展望台、伊雑宮/猿田彥路線建議

### 2026-05-01 v1 初始版本

- 4 區域插畫 banner（BOSS 親選版本）
- 49 景點 + 32 家美食
- Anti AI-slop 設計風格
- GitHub Pages 部署

---

## 待開發項目

- [ ] 手機版漢堡選單
- [ ] 區域間交通串接建議
- [ ] 景點實際照片替換 SVG 圖示
- [ ] 天氣/季節推薦提示
- [ ] 多語系支援（日文/英文切換）
- [ ] 旅程天數規劃建議（1-5 天行程）
