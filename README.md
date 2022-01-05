<p align="center">
    <a href="https://github.com/yiisoft" target="_blank">
        <img src="https://avatars0.githubusercontent.com/u/993323" height="100px">
    </a>
    <h1 align="center">Testing some git command lines in Yii2 Basic App</h1>
    <br>
</p>

Yii 2 Basic Project Template is a skeleton [Yii 2](http://www.yiiframework.com/) application best for
rapidly creating small projects.

The purpose of the repository is to practice some Git command lines to stop tracking a files or folders that have been tracked in the origin repo.

###Untrack change locally and conserve the file in original repository
We can update local git repository by running following command:

```git update-index --assume-unchanged <file>```

In this case a file is being tracked in the origin repo. You can modify it in your local repo and git will never mark it as changed.
To revert the effect of this command, run the following command:

```git update-index --no-assume-unchanged <file>```

###Stop tracking and Remove from the original repository but not local
If we stop tracking a file or folder that have been tracked in the initial commit or something like that and 
this file exists in the original repository **(example: node_modules)** and we want to remove it 
from repository, the following command can help us:

IMPORTANT! -> Make changes you want in .gitignore file first. 

```git rm -r --cached .```

to remove all files from git cache

```git add .```

to add all files again

```git commit -m "Commit message"``` 

or just  

```git commit```

or continue working.

