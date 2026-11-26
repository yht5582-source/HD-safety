# HD-safety｜透析安全整合管理

版本：v0.4。整合床位燈號、CFS 引導評估、60 床模擬資料與互動疏散演練地圖。

目標網站：https://yht5582-source.github.io/HD-safety/

## 功能

- 床位總覽：臨床血壓燈號、接手及複測紀錄。
- 衰弱與照護：CFS 分類引導、臨床確認、評估歷史與下次追蹤日期。
- 疏散演練地圖：預載三樓平面圖，定位床位、標示安全區、繪製演練路線，追蹤離機、調度、抵達與點名。
- 60 床模擬資料；臨床燈號、CFS 與當次疏散需求分開管理。

## GitHub Pages 發布

1. 開啟 https://github.com/yht5582-source/HD-safety/upload/main ，上傳本資料夾內的 `index.html` 與 `README.md`，提交至 `main`。若是空儲存庫，先由首頁的「uploading an existing file」進入上傳頁。
2. 開啟 https://github.com/yht5582-source/HD-safety/settings/pages 。
3. Source 選 **Deploy from a branch**；Branch 選 **main**，資料夾選 **/ (root)**，按 **Save**。
4. 等待 Pages 建置成功，再開啟目標網站。未成功發布前，目標網站可能顯示 404。

本網站為單一靜態 HTML，不需要安裝套件或執行編譯；更新時替換根目錄 `index.html` 即可。

## 使用

可先從床位總覽選擇病人，再到「衰弱與照護」填寫評估。完成必要作答後顯示建議 CFS，臨床確認後才套用至床位。穩定者預設每6個月追蹤，事件恢復後可選2–3個月。

疏散模組預載林麗珍11/25回傳的三樓平面圖。請團隊實地確認床號、可用通道、安全區及演練路線；系統不自動決定撤離優先順序。配置 JSON 不包含底圖、病人資料或演練進度；重新開啟時需配合相同底圖載入配置。

## 資料與使用範圍

示範資料非真實病人紀錄，請勿在公開示範網站輸入真實個資。此版未介接院內電子透析系統，也不是已驗證的 AI 低血壓預測模型。評估、處置與疏散均需依院內核定流程與現場判斷。

## 參考資料

- [KDIGO 血壓與體液管理共識](https://pmc.ncbi.nlm.nih.gov/articles/PMC7215236/)
- [Clinical Frailty Scale 原作者說明](https://www.dal.ca/sites/gmr/our-tools/clinical-frailty-scale.html)
- [Theou et al. CFS classification tree](https://doi.org/10.1093/ageing/afab006)
- [2026 CKD 衰弱管理共識](https://www.nature.com/articles/s41581-026-01128-3)

## 本次發布狀態

2026-11-26：已確認目標儲存庫存在，並準備本部署檔。自動上傳遭執行環境的核准政策阻擋，尚未寫入 GitHub，也尚未驗證 Pages 上線。
