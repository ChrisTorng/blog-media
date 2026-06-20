# blog-media

本資料夾使用 `http-server` 提供本機開發所需的媒體檔案。

## 啟動伺服器

在本資料夾執行：

```powershell
npm start
```

接著開啟 <http://127.0.0.1:3001/>。

伺服器設定儲存在 `package.json`：固定使用 port `3001`、只監聽本機，並停用快取以方便開發。`http-server` 需已安裝並可由終端機直接執行。
