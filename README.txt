Scratch 選手觀察日誌 v1.0

這是靜態網頁 App，不需要付 Apple 開發者年費。內含 4 位選手、6 項評分、課堂歷史、兩次課程比較、JSON 備份還原與 CSV 匯出。每次評分或輸入都儲存於本機 localStorage。

部署：建立新的 GitHub repository（例如 scratch-observer），上傳本資料夾內的 index.html、manifest.webmanifest、sw.js、icon.png、icon512.png 至根目錄。Settings > Pages > Deploy from a branch > main / (root) > Save。待 Pages 網址顯示後，用 iPhone Safari 開啟，分享 > 加入主畫面 > 作為網頁 App 開啟。第一次在主畫面 App 開啟並確認可用，再輸入正式資料。網站程式碼可公開，但切勿上傳學生名單、備份或紀錄。也可使用學校核准的 HTTPS 靜態網站。

電腦可先以瀏覽器開啟 index.html 試用；本機檔案網址的儲存行為因瀏覽器而異，正式紀錄請使用固定 HTTPS 網址與同一個主畫面 App。首次連線成功後，service worker 將快取程式檔案，離線可用性仍須在實機測試。沒有雲端同步；清除網站資料或移除 App 可能遺失紀錄。請定期匯出 JSON 到受保護的檔案空間，CSV 可另用 Excel 分析。JSON 匯入會在確認後取代現有紀錄。

教師紀錄不應與學生共用。請使用代號、手機鎖定、學校核准的儲存方式。此版本尚未於 iPhone Duo 實機測試。
