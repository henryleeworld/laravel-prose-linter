# Laravel 8 散文程式碼規範檢查工具

引入 beyondcode 的 laravel-prose-linter 套件來擴增散文程式碼規範檢查工具，幫助潤色應用程式的文本，讓工具檢查您的翻譯，甚至檢查您的 Blade 模板是否存在拼寫錯誤、俚語，並根據您選擇的散文風格獲得更好的寫作風格的建議。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan lint:{檢查內容}
```

----

## 畫面截圖
![](https://i.imgur.com/A2GpJcY.png)
> 檢查特定的翻譯命名空間