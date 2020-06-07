# Install Hugo in Cloud9

***Assumptions:***  
*- Cloud9 is configured*  
---

Download and install Hugo and add it to path directory:
```
curl -s https://api.github.com/repos/gohugoio/hugo/releases/latest | grep browser_download_url | grep Linux-64bit.tar.gz | cut -d '"' -f 4 | wget -q -i - -O - | tar xvz -C ~/bin hugo
```
---
Verify install:
```
hugo version
```
---
**Resources:**  
https://blog.atj.me/2018/04/cloud9-with-a-chance-of-hugo/