# about_us

> Introduction of SB team

## 環境設定

1. Fork這份專案後，在home目錄下執行` git clone + 你的專案url `。
2. 移動至`AboutUsSB`後，執行` npm i `。
3. 移動至`AboutUsSB`底下的 `config`後，用編輯器開啟 ` index.js ` 
4. 你會看到:
```
'use strict'
// Template version: 1.3.1
// see http://vuejs-templates.github.io/webpack for documentation.

const path = require('path')

module.exports = {
  dev: {

    // Paths
    assetsSubDirectory: 'static',
    assetsPublicPath: '/',
    proxyTable: {},

    // Various Dev Server settings
    host: 'localhost', 
    port: 8080, // can be overwritten by process.env.PORT, if port is in use, a free one will be determined
    .....
```
  請將```port: 數字 ``` 改成你喜歡的數字後，儲存。  
  
5. 回到`AboutUsSB`目錄，執行` npm start ` 就可以打開另外一個terminal開始編輯。如果有語法錯誤也會在這個terminal顯示。
6. 在自己的電腦開啟「 `http://luffy.ee.ncku.edu.tw:你剛剛輸入的數字/#/` 」就可以看到結果。
