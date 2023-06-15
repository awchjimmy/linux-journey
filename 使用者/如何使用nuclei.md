# 如何使用 nuclei

### 多個 hosts，一個 template
```sh
nuclei -l "urls.txt" -t "http/default-logins/geoserver/geoserver-default-login.yaml"
```
