# Configure New Cloud9 Environment


Install Cloud9 CLI:
```
npm install -g c9
```
---
Verify Cloud9 CLI:
```
c9 --help
```
---
Set git name and email in .gitconfig:
```
git config --global user.name "Richard Vass"
git config --global user.name rvass@icloud.com
```
---
Set git to use the credential memory cache. Default timeout is 15 minutes.
```
git config --global credential.helper cache
```
Set credential helper to 10 hours
```
git config --global credential.helper 'cache --timeout=36000'
```
---
Verify .gitconfig settings
```
cat ~/.gitconfig
```
---
Create the /bin directory
```
mkdir ~/bin
```
---
**Resources:**  
https://cloud9-sdk.readme.io/docs/the-cloud9-cli