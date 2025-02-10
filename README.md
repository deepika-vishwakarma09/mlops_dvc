# mlops_dvc
complete dvc with git

dvc remote add -d myremote1(iska naam apne tarike se change kr skte h) S3

dvc add data(for tracking all file we write folder name or only write that file name)/  {commond for adding data}


output 'data' is already tracked by SCM (e.g. Git).(when git tracked data folder then error occurs)
    You can remove it from Git, then add to DVC.
        To stop tracking from Git:
            git rm -r --cached 'data'(we use this commond to stop tracking from git ### where data is name of folder)
            git commit -m "stop tracking data"(after stoping track we commit)

{PS C:\Users\DIPIKA VISHWAKARMA\Desktop\mlops\mlops_dvc>  git rm -r --cached 'data'
rm 'data/sample_data.csv'
PS C:\Users\DIPIKA VISHWAKARMA\Desktop\mlops\mlops_dvc> git commit -m "stop tracking data"        
[main 8860b47] stop tracking data
 4 files changed, 6 insertions(+), 4 deletions(-)
 create mode 100644 .dvc/.gitignore
 create mode 100644 .dvc/config
 create mode 100644 .dvcignore
 delete mode 100644 data/sample_data.csv
PS C:\Users\DIPIKA VISHWAKARMA\Desktop\mlops\mlops_dvc> }