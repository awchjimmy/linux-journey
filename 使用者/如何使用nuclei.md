# 如何使用 nuclei

### 列出可用 template 清單
```sh
nuclei -tl
```

### 多個 hosts，一個 template
```sh
nuclei -l "urls.txt" -t "http/default-logins/geoserver/geoserver-default-login.yaml"
```
