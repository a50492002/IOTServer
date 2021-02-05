# Tools

### 利用venv建立Python虛擬環境 並安裝相依性套件
```
py -m venv .env
.env\scripts\activate.ps1
pip install -r requirements.txt
```
###### .env命名請正確 git上簽同步的時候會自動省略虛擬環境

### 解決 xxx.ps1 檔案無法載入問題
###### 如果無法啟動 activate.ps1 請以管理員身分打開PowerShell 執行 
    set-executionpolicy remotesigned
###### 選擇 [Y]:是 (按下Y鍵後Enter)

## Python 套件相依性管理

### 建立套件相依性檔案
    py -m pip freeze > requirements.txt

### PIP 安裝套件相依性檔案的套件
    py -m pip install -r requirements.txt

## 本機端啟動開發網頁服務
### 啟動測試環境
    .env\scripts\activate.ps1

### 啟動開發用網頁伺服器
    py WebTools/manage.py runserver
###### "c:/.../" 為你的專案存放路徑
