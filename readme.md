# About
Data Version Control (DVC) 
Input Images versions for ML model training are being versioned

Google Drive has been used as Backend to store the objects 

High level commands:
*Note: For your project/repo change the values corresponding to Git and GDrive* 
```commandline
Data Versioning - DVC Commands

1. Create DVC folder
2. Create FOLDER with artifacts
3. Run > git init
4. Run > dvc init
5. dvc add $FOLDER .gitignore
6. Verify files inside - cd .dvc/cache


##Install Google Drive module
pip install dvc_gdrive

##Manually creeate folder in your Google Drive and use reference as shown below
dvc remote add --default myremote gdrive://1tv-FsXKnjef6y7lfMKyGIMAdrR_ItusDAA
dvc remote modify myremote gdrive_acknowledge_abuse true

##Autheticate yourself 
dvc push

#Track DVC config in GIT
Create GIT Repo at github.com
echo .dvc/cache >> .gitignore
git add --all
git commit -m"Adding initial DVC tracking files into GIT"
git branch -M master
git remote add origin git@github.com:say2imran/DVC-sample-images.git
git push -u origin master

```


