# GitHub Cloning and Feature braching

## How?

Follow simple steps as listed below and I will explain this in person as it might need some help.

\* NOTE: **_security_aggregation_** is a sample repository for explaining the following. Please don't assume anything. 

1. Ensure you installed Git command line tool or any client that you favor for _Gitting_

2. Clone using your forked repository (this will create a folder **security_aggregation**): 
```
git clone https://github.com/<your_git_username>/security_aggregation.git
```

3. Go to newly created branch in your local path:
```
cd security_aggregation
```

4. Add _upstream_ or original repository:
```
git remote add upstream https://github.com/jhulfikarali/foo.git
```

5. Sync your fork repository (syncs up your forked repository against upstream repository):
``` 
git pull --rebase master upstream master
git push origin
```
6. Feature branch (this creates a new tree/branch with the name _new\_feature_, usually this can be your request/bug/JIRA ticket #):
```
git checkout -b new_feature
```

7. Do your stuff in the code to create something cool!! 
```
print("Hello world, GitHub!")
### Just for fun... Do your coding art.
```

8. Add updated files for commit log (please note that below adds all changed files but you can pick one file or any wildcard):
```
git add *
```

9. Commit the changes:
```
git commit -m "Changed the world! Wait, just hello world right??? Huh!!!"
```

10. **Are we done?** This is where I lost when i came from SVN/SubVersion. Please note that, this commit is just local to your desktop system.

11. Git push - Push the changes to repository (_fork_):
```
git push origin _new\_feature_
```
> This will send your changes to you GitHub repository.

12. Based on your project setup, above step might [create a PR](https://github.com/jhulfikarali/learning/blob/master/Git_PR.md) or merge the changes to upstream repository.

And you are done for now!!!!

[Learning HomePage](https://github.com/jhulfikarali/learning)
