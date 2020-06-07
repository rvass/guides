# New Hugo Project in Cloud9

***Assumptions:***  
*- Cloud9 is configured*  
*- Hugo is installed in the /bin*

---

Create and initialise new Hugo project directory
```
hugo new site quickstart
```

Add a theme:
```
cd quickstart  
git init  
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
```
Add the theme to the site config file:
```
echo 'theme = "ananke"' >> config.toml
```  
Add some content:
```
hugo new posts/my-first-post.md
```
---
**Resources**  
https://blog.atj.me/2018/04/cloud9-with-a-chance-of-hugo/  
https://gohugo.io/getting-started/quick-start/