# 北陸・中部 攝影旅遊指南 — 開發進度

## 專案資訊

- **本地路徑**：`/home/james/PROJECT_REBOOT/hokuriku-travel-site/`
- **GitHub Repo**：`2pistudiojames-lang/hokuriku-travel`
- **GitHub Pages**：https://2pistudiojames-lang.github.io/hokuriku-travel/
- **LAN 預覽**：http://192.168.1.115:4195/（systemd user service）
- **GitHub 帳號**：2pistudio.james@gmail.com / username: 2pistudiojames-lang
- **Repo 可見性**：Public（GitHub Pages 免費方案要求）

---

## 更新發佈流程

```bash
cd /home/james/PROJECT_REBOOT/hokuriku-travel-site

# 1. 查看變更
git status

# 2. 加入所有變更
git add -A

# 3. 提交（寫清楚改了什麼）
git commit -m "描述這次改了什麼"

# 4. 推送（GitHub Pages 會自動部署，約 30 秒生效）
git push
```

### 注意事項
- Token 已存在於 git remote URL 中，`git push` 無需再輸入密碼
- GitHub Pages 部署通常 15-60 秒，Push 後稍等再確認
- LAN 預覽服務為 `hokuriku-travel-preview.service`，即時反映本地檔案變更
- 建議開發時先用 LAN 預覽確認，沒問題再 `git push`

---

## 開發里程碑

### 2026-05-01 v1 初始版本

**設計基礎**
- 參考 `zenkojidaira.or.jp` 視覺風格
- 自然色系（Teal、橄欖、深藍、赤褐、金沙）
- Noto Serif JP 標題 + Noto Sans TC 內文
- Anti AI-slop Rules：無漸層、無 icon spam、內容 > 裝飾

**4 區域攝影景點**
- 金澤 14 景點（兼六園、東茶屋街、近江町市場等）
- 富山 14 景點（雨晴海岸、環水公園、庄川峽等）
- 名古屋・犬山・岐阜 14 景點（名古屋城、犬山城、鵜飼等）
- 伊勢 7 景點（伊勢神宮、夫婦岩、鳥羽等）
- 共 49 個景點，每個含拍攝時段、建議鏡頭、攝影重點

**插畫 Banner**
- 金澤：BOSS 提供（兼六園、城郭、市場、和菓子）
- 富山：BOSS 提供（立山連峰、富山灣、海鮮、雪之大谷）
- 名古屋：BOSS 提供（名古屋城、鵜飼、鰻魚飯）
- 伊勢：BOSS 提供（神宮鳥居、夫婦岩、海濱町）
- 統一圓角 banner + shadow + lazy loading

**必吃美食（各 8 家）**
- 金澤 8 家：福井家、金沢おでん 彩、谷中葱 ぼたん、はしまきや、うら田、森八、中田屋、金沢牛亭
- 富山 8 家：大喜、白えび亭、氷見うどん 源、ひまわり、銀兵、ケーキハウス・タカマツ、クロッキー、旭壽司
- 名古屋 8 家：あつた蓬莱軒、矢場とん、天むす 千寿、喫茶マリーン、世界の山ちゃん、コンパル、蓬莱軒松坂屋店、伏見フルーツガーデン
- 伊勢 8 家：赤福本店、冨田屋、山田ふくすけ、すし久、二軒茶屋餅、伊勢萬、豆腐庵、伊勢神職茶屋
- 店名可複製、點擊開 Google Maps

**部署**
- GitHub Pages 啟用（legacy 模式，main branch root）
- LAN 預覽服務 `hokuriku-travel-preview.service`（port 4195）

---

## 待開發項目（Future Ideas）

- [ ] 手機版漢堡選單（目前 nav 在小螢幕可能過擠）
- [ ] 區域間交通串接建議
- [ ] 景點實際照片替換 SVG 圖示
- [ ] 加入天氣/季節推薦提示
- [ ] 多語系支援（日文/英文切換）
- [ ] 加入旅程天數規劃建議（1-5 天行程）
