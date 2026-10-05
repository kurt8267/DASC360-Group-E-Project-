# Welcome to the DASC360 Group E Project GitHub

To get started please install the following software:
- [Visual Studio Code](https://code.visualstudio.com/download)
- [GitHub Desktop](https://desktop.github.com/download/)

One both are installed, please add the following extensions to Visual Studio Code:
- [Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)
- [R](https://marketplace.visualstudio.com/items?itemName=REditorSupport.r)

We are using the ["clone, fetch, pull, and push"](https://marketplace.visualstudio.com/items?itemName=REditorSupport.r) Git workflow. Here are important terms:
- **Repository:** The online files hosted by GitHub, like a OneDrive folder.
- **Clone:** Creating a local copy of the files in the repository.
- **Branch:** a specific version of the files you are working on. <u>Always make a new branch to work on and never edit an existing branch.</u>
- **Commit:** Saving the changes you have made to your local clone.
- **Push:** Updating the online repository to match your local commit.
- **Merge:** Combining the changes across two branches. If you want to edit an existing branch, always make a new branch to work on then merge the two at the end.

### Getting R to Work in VS Code
Follow these instructions:
1. Find your installation of R. This is easiest by opening RStudio and running the command `R.home()`. For me this command returns `"C:/Users/john4207/AppData/Local/Programs/R/R-4.6.1"`
2. Add your R folder to system path. Type `env` into the Windows search bar, select `Edit the system environment variables` and at the bottom of `Advanced` click `Environment Variables`. Double click `PATH`, then click `New` and in an empty row add the path to the R directory. For me `C:\Users\john4207\AppData\Local\Programs\R`
3. Install language server. Open the R.exe file in your installation directory, for me it is at `C:/Users/john4207/AppData/Local/Programs/R/R-4.6.1/bin/R.exe` then run the command `install.packages("languageserver")`. This command must be run through this .exe file and not RStudio or it won't work.
4. Add the R.exe path to VS Code. Open the extensions window, select the [R](https://marketplace.visualstudio.com/items?itemName=REditorSupport.r) extension, click the gear, click settings. Paste the R.exe path you just ran into `R: Console Path` and `R: Executable Path`
5. Try to run some R code in VS Studio. You may get an error message asking you to download SESS, if you do click download. It should work now.
6. Congratulations! You have completed the bizarrely difficult process to get R to work in VS Code!