# 如何使用 nuclei

### 列出可用 template 清單
```sh
nuclei -tl
```

### 多個 hosts，一個 template
```sh
nuclei -l "urls.txt" -t "http/default-logins/geoserver/geoserver-default-login.yaml"
```

### 範例：從 header 看 IIS 版本
```sh
nuclei -l "urls.txt" -t "http/technologies/microsoft/microsoft-iis-version.yaml"
```

### 範例：找 geoserver 預設帳號密碼
```sh
nuclei -l "urls.txt" -t "http/default-logins/geoserver/geoserver-default-login.yaml"
```

### 範例：找 Swagger API 文件
```sh
nuclei -l "urls.txt" -t "http/exposures/apis/swagger-api.yaml"
```

### 範例：找 遠端桌面連線
```sh
nuclei -u 211.75.103.196 -t network/detection/rdp-detect.yaml
```

### 範例：找 wordpress 網站
```sh
nuclei -l "urls.txt" -t http/vulnerabilities/wordpress/wp-license-file.yaml
```
