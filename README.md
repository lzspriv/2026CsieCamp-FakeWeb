# 2026CsieCamp-FakeWeb

本專案為 **NTNU CSIE Camp（師大資工營）教學示範用靜態網站**，用途是宣導「識讀網域的重要性」：不能因為網站外觀相似或可正常點擊進入，就直接判定該網站為真實可信來源。

> 僅供教學使用，不作為正式對外網站。

## 專案目標

- 透過仿真頁面情境，提醒使用者辨識可疑網域與釣魚風險
- 強調「外觀相同不代表來源可信」的網路安全觀念

請特別注意：**判斷網站真偽時，應優先檢查完整網域名稱（Domain）**，而不是只看頁面外觀是否相似。

## 教學部署網域

本專案目前部署於以下兩個網址，作為網域識讀教學對照案例：

- https://www.csie.ntnu.edu.tw/
- https://www.csie.ntnu.eud.one/

## 搜尋引擎收錄防護（請勿移除）

為避免教學用假網站出現在搜尋結果中，專案已加入以下設定：

- 根目錄 [robots.txt](robots.txt)：
	- `User-agent: *`
	- `Disallow: /`
- 首頁 [index.html](index.html) `<head>`：
	- `<meta name="robots" content="noindex, nofollow, noarchive, nosnippet, noimageindex">`
	- `<meta name="googlebot" content="noindex, nofollow, noarchive, nosnippet, noimageindex">`

請勿在教學期間移除上述設定，以降低本頁面被搜尋引擎收錄或保留摘要的機率。
