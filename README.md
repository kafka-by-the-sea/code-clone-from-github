* 開發環境: 我自己是使用 Mac OS, Windows/Linux請自行google環境安裝教學
* Web Server: 請依自己的習慣自行安裝，例如：使用Apache, Nginx ...
* 如果你需要從這裡下載專案，請依照下列步驟還原專案

## Native PHP Code
1. 請確認本機端已經安裝PHP
2. 請確認本機端已經安裝composer
    * https://getcomposer.org/
3. git clone 專案
```
git clone https://github.com/monkeypg/mapping-to-assoc.git
```
4. 還原vendor目錄
```
composer install
```

## Laravel 專案
1. 請確認本機端已經安裝PHP & MySQL
2. 請確認本機端已經安裝composer
3. git clone 專案
```
git clone https://github.com/monkeypg/laravel-books-API.git
```
4. 還原vendor目錄
```
composer install
```
5. 還原.env
```
cp .env.example .env
php artisan key:generate
```
* .env裡面是本機端的MySQL帳號與密碼
* 因為.env.example的APP_KEY為SomeRandomString，必須下php artisan key:generate重新產生APP_KEY。
6. 重建資料庫
* 請在專案目錄下，做migration與seeder
```
php artisan migrate
php artisan db:seed(依程式碼內容而定，請看Laravel文件，了解如何使用seed，不要直接貼上指令)
```
## Python
1. 使用Python 3
2. 請自行google如何安裝Anaconda
