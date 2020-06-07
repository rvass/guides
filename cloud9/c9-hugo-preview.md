# Previewing Hugo Changes in Cloud9

***Assumptions:***  
*- Cloud9 is configured*  
*- Hugo is installed in the /bin*  
*- A hugo project with content has been created*
*- working directory is /project*
---
1. Navigate to project directory:  
```
cd project-directory
```
2. Click on *Preview > Preview Running Application*.    You will be greeted by an “Oops” message because the hugo server is not running.  
  
3. Open the Cloud9 Preview tab in an external firefox tab and copy the URL to the clipboard.  
  
4. Start the hugo server with the following arguments (use the preview URL in place of PREVIEW_URL):
```
hugo serve --bind=0.0.0.0 -p 8080 -b PREVIEW_URL --appendPort=false --disableFastRender
```
5. Click Run > Run Configurations > New Run Configuration
6. In the box next to Run and Restart, type the name that will display on the Run, Run Configurations menu for this run configuration. 
7. In the Command box, type any custom command line options you want to use. 
8. To have this run configuration use a specific working directory, choose CWD, choose the directory to use, and then choose Select. 
---
**Resources**  
https://blog.atj.me/2018/04/cloud9-with-a-chance-of-hugo/  
https://docs.aws.amazon.com/cloud9/latest/user-guide/build-run-debug.html