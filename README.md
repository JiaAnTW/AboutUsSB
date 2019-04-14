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

## 專案結構
* build
* dist: 
  >編譯後出現，也是之後要上傳的資料夾
* config
* node_modules 
  >npm i後出現，用來存npm載下來的套件
* src:
  > 編譯前程式碼位置，也是我們**寫code的地方**
  * App.vue: 
      >讓我們所寫的vue填入html檔，不用修改
  * Index.vue:
      >控制首頁的地方，這次擔任**所有組件的控制中心**
  * asset:
      >放素材的地方(圖片、音樂.......)
  * components:
      >放組件的程式碼
      * Landing.vue
      * Team.vue
      * SelfIntro.vue
      * Profile.vue
  * router: 
    >控制路由(定義不同網址所導向的頁面)的地方，這次不會用到 
* static
* test
