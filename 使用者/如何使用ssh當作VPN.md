# 如何使用 ssh 當作 VPN

> 以下用「本機」與「跳板機」區分二台機器。

### 跳板機：確認跳板機有 ssh server
略，若沒有請直接連絡管理者。

### 本機：建立 ssh tunnel
```
ssh -D 2323 awchjimmy@170.187.227.8
```

### 本機：Chrome 啟動參數
```
--proxy-server="socks5://localhost:2323"
```

### 本機：檢查 IP
檢查 IP 即可知道是否跳板成功。
