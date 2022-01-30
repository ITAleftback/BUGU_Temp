# BUGU_Temp

*本仓库为不咕平台的临时仓库，未来将会被移动到服务器仓库中。*

## 加入项目

请各位按照如下方法来参与项目：

1. 在github的本项目中`Fork`本仓库，并`clone`你所`Fork`的副本，以便未来向本仓库提交`pull request`。

2. 进入你所`clone`的本地副本，使用`git switch -c develop origin/develop`使用`develop`分支进行开发。

3. 根据你目前所进行的阶段性任务，新建一个自定义的分支`git switch -c <name>`，当前你所执行的所有任务请在本分支内进行。

4. 当你完成了一个阶段性任务，此时请将其合并至你的`develop`分支中，并`push`到你的仓库同时提交`pull request`等待主仓库的合并。

5. 主仓库的`develop`仓库将长期持续进行合并，而在完成了某一项完整功能后，`develop`仓库将合并至`release`仓库以进行发布前的检查。

6. 当检查完毕后，`release`仓库将会合并至`master`仓库完成一次版本更新。

7. 请注意以上步骤，同时，若本人在本地进行开发请始终使用自建分支进行工作，如果是在进行功能开发，请将合并提交至`develop`，如果是进行bug修复，请将合并提交至`release`，使用`release`分支的方法同`develop`。在没有申请或要求的情况下，请勿向`master`分支提供合并。

8. 请注意写明`commit`时的注释，同时`pull request`也需要说明详情，另外在编程中的注释请一律规范使用中文且尽量多添加注释。

## 分组合作

1. 当前仓库工作区根目录下有四个文件夹：
   
   1. `data`：数据文件夹，用于存放一些数据文件。
   
   2. `log`：日志文件夹，用于存放日志文件，也可以存放各位的一些工作记录或临时笔记。
   
   3. `workspace`：工作文件夹，主要工作区。
   
   4. `preference`：参考文件夹，用于存放一些文档说明文件。

2. 上述每个文件夹下均有：
   
   1. `back`：后端
   
   2. `front`：前端
   
   3. `embedded`：嵌入式
   
   请各位按照自己的分组在规定文件夹下工作。

3. 在`log`文件夹下属于自己的分组文件夹中，可以新建一个文件夹并为其命名，该文件夹将可以作为你的工作笔记存放处，但请在分组文件夹的`README.md`文件中进行说明。

4. 当组内需要在工作区根至三级目录新建任何新文件夹，均应在该文件夹下的`README.md`中记录该文件夹的功能或作用，可以查看`./log/embedded/README.md`文件作为示例，三级目录之后暂时可以不添加。

## 开发规范

### commit

在提交commit的时候请尽量遵守本规范以提高大家commit的可读性，之前已经提交过commit可以不管，但在本规范提出后请尽量遵守。

- 尽量使用`git commit`而非`git commit -m <message>`来提交，使用前者git将打开你的默认git编辑器，此间你可以在该编辑器中进行更加方便完整的多行书写。如果你的git使用了一个你不熟悉的编辑器，可以选择换掉它，因为每人熟悉的编辑器各不相同，故具体方法请自行百度。

- 在编辑器中，请按如下方式进行编写commit:
  
  ```git
  修改类型：简述修改
  # 注意此处应有一行空行
  介绍修改
  ```
  
  上述方法中，`介绍修改`为可选项，`修改类型`和`简述修改`为必选项。
  
  其中`修改类型`有：
  
  - `功能`：新功能
  
  - `修复`：修补bug
  
  - `文档`：修改文档
  
  - `格式`：除上述外任何不影响代码运行的修改
  
  - `重构`：非新功能，也非bug修补
  
  - `微调`：非上述修改的任何调整
  
  - `测试`：增加测试

在`简述修改`中，请在一句话内概括本次修改的内容。

在`介绍修改`中，可以用多行文字描述本次修改的内容、目的以及其它内容。

- 当发现本次修改的内容太多无法一次性用一个`修改类型`或一句话内的`简述修改`进行描述时，请重新规划`git add <file>`进行原子提交，通过多次提交的方式完成上述规则。

- 在提交过程中，除专业词语外，如无必须，请使用中文进行描述以便更加准确明了。

## 开发环境安装

- [嵌入式](./preference/embedded/install.md)

## 资料汇总

考虑到各位对集体开发尚缺少经验（包括我也是），所以大家可以将自己搜集到的认为有价值的资料放至此处：

- [git一些常用指令汇总](https://yunwuhai.blog.csdn.net/article/details/122515950)

- [github如何上传自己的代码到自己的仓库和到别人的仓库](https://blog.csdn.net/weixin_43851149/article/details/107283174)

- [github简明指南](http://rogerdudler.github.io/git-guide/index.zh.html)

- [像git一样思考](http://think-like-a-git.net/)

- [github如何同步主仓库到自己的fork仓库](https://blog.csdn.net/dingjianmin/article/details/117393092?utm_medium=distribute.pc_aggpage_search_result.none-task-blog-2~aggregatepage~first_rank_ecpm_v1~rank_v31_ecpm-1-117393092.pc_agg_new_rank&utm_term=%E5%A6%82%E4%BD%95%E5%B0%86%E8%87%AA%E5%B7%B1%E7%9A%84fork%E6%9B%B4%E6%96%B0&spm=1000.2123.3001.4430)

- [编译原理网课](https://www.bilibili.com/video/BV1zW411t7YE?from=search&seid=13066746962877628745&spm_id_from=333.337.0.0)

## 项目规划
