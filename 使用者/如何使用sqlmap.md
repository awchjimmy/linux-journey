# 如何使用 sqlmap

### 檢查 sqlmap 有沒有安裝
```sh
sqlmap --version
```

### 指定目標，後面加 -u
```sh
sqlmap -u "https://www.taipower.com.tw/TC/page.aspx?mid=44"
```

### 手動指定參數位置，後面加*
```sh
sqlmap -u "https://iest.taipower.com.tw/Home/PublicationDetail/32*"
```

### 用預設答案回答所有 sqlmap 問題，後面加 --batch
```sh
sqlmap -u "https://www.taipower.com.tw/TC/page.aspx?mid=44" --batch
```
