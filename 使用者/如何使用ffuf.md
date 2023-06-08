# 如何使用 ffuf

### 前言
ffuf 只適合做極簡單的一個動作，超過一個動作時，請自行寫 python 程式。

**適合**：一個 GET / 一個 POST

**不適合**：解 CSRF token、邏輯判斷、解reCAPTCHA

用不適合的工具，所花費的時間划不來！

### 使用 ffuf
```
ffuf -w "./wordlist.txt" -u "https://example.com/FUZZ"
```

### 存檔到特定資料夾
```
ffuf -w "./wordlist.txt" -u "https://example.com/FUZZ" -od out/
```
