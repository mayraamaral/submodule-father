# Git & Github Submodules
A submodule is a git repository linked to another one. As example, this is the "father" repository and the folder inside this repository is the "child".  
  
To start a submodule, you just have to enter the father repository and type:  
  
```git submodule add https://github.com/${USERNAME}/${NAME_OF_THE_REPOSITORY}```  
  
The integration between commits isn't synchronous, every time you push a commit, you also have to bring it to the father repository. You can do it this way:  
  
```git submodule foreach git pull origin main```  
  
Maybe this can also be helpful:  
  
- [Article on Github blog](https://github.blog/2016-02-01-working-with-submodules/)  
- [Issue on Github about Git submodules and integration](https://github.com/tj/git-extras/pull/80)