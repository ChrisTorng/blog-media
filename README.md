# blog-media

網站文章的音訊與影片存放在這個 repo，正式網址是 <https://media.christorng.idv.tw>。

## 啟動本機伺服器

在本資料夾執行：

```powershell
npm start
```

接著可從 <http://localhost:3001/> 存取檔案。伺服器固定使用 port `3001`、只監聽本機，並停用快取。

主網站內容使用 `/blog-media/<path-from-repo-root>` 路徑。例如，本 repo 的 `audio/example.mp3` 在內容中寫成 `/blog-media/audio/example.mp3`。主網站元件會在開發環境解析成 `http://localhost:3001/audio/example.mp3`，在 production 解析成 `https://media.christorng.idv.tw/audio/example.mp3`。

`http-server` 需已安裝並可由終端機直接執行。
