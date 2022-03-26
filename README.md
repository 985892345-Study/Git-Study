
[TOC]
> ***由于使用 Typora 进行编写，所以有些格式不同，建议 clone 下来使用 Typora 进行查看***

# 图形化使用 Git 的保姆级教程

## Github Desktop

> 由于很多学弟刚开始学习命令行有些难度，所以这里对 github 的图形化操作进行讲解。
>
> 图形化虽然简单，但命令行也是非常重要的，强烈建议各位学习一下命令行的使用
>
> 注：本教程需要一定 git 基础，且教程内不会教什么是 commit、add、push 等作用，这些请自己学习 git 指令
>
> 还没学习 git 指令的请[点我](#git学习推荐网站)

> 你说 idea 可以 Github Desktop 的所有操作，为什么还要 Github Desktop？
>
> 因为 idea 里的 GitHub 插件经常有一些玄学问题，在后面我会指出

### 下载

> 建议使用 edge 或者 Google Chrome

百度搜索 Github Desktop 或者点击 https://desktop.github.com/ 进行下载

### 登录

1、点击Sign in 打开浏览器登录，如果登录打不开，多半是强，请看[改host](#改host访问github)

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211020192222298.png" alt="image-20211020194102498" style="zoom:40%;" />

2、登陆后这里建议更换邮箱为自己注册 github 时的邮箱(点击右边向下箭头)

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211020193744614.png" alt="image-20211020193744614" style="zoom:50%;" />

3、进入这个界面就🆗了

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211020194102498.png" alt="image-20211020192222298" style="zoom:33%;" />

### 创建本地仓库

1、点击左上角 File - Add local repository

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211020194311766.png" alt="image-20211020194311766" style="zoom:50%;" />

> 学长，创建本地仓库为什么不点第一个 New repository?
>
> 其实点第一个也行，但有些坑，第一个更偏向用于创建一个只带有.git文件的空的文件夹，如果想用它来指向你的项目文件夹，需要你手动输入项目文件夹的全名。而第二个就可以直接省去这些步骤。

2、点击 Choose 然后选择你的项目文件夹

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211020195540651.png" alt="image-20211020195540651" style="zoom:50%;" />

> 例如我有一个叫 Test 的项目，就选择他就 OK（别选到里面的 src 这些，我们需要的是整个项目文件）
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211020195416879.png" alt="image-20211020195416879" style="zoom: 50%;" />

3、然后点击 create a repository 创建本地仓库

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211020202240883.png" alt="image-20211020202240883" style="zoom:50%;" />

4、描述和README

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211020203558784.png" alt="image-20211020203558784" style="zoom:50%;" />

5、到这里你的本地仓库就创建完了

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211020200657266.png" alt="image-20211020200657266" style="zoom:50%;" />

> 学长，提交是什么意思？
>
> 提交是 commit，但如果不知道，请先了解 git 指令！



### 创建云端仓库

> 之前我们已经成功创建了本地仓库，接下来将带你创建云端仓库

1、上传本地仓库至 Github，点击下图所示

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022214611182.png" alt="image-20211023005207748" style="zoom:50%;" />

2、在这里有一个坑，它默认云端仓库是 private，视自己情况可以选择关闭这个选项（但发给我们的作业必须关闭这个）

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022214855455.png" alt="image-20211022214855455" style="zoom:50%;" />

3.1、出现下图一般是墙的问题，这个请看[改host](#改 host 访问 Github)

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023005301191.png" alt="image-20211022214611182" style="zoom: 50%;" />

3.2、当左下角的 Initial commit 没有的时候，恭喜你上传成功，接下来点击 View on Github 打开 github（可以记下这个快捷打开方式）

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022220705131.png" alt="image-20211023010229811" style="zoom:50%;" />

4、成功的界面

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023005207748.png" alt="image-20211022221020408" style="zoom:25%;" />



### 更方便的clone

> 有了 Github Desktop 后，在 github 中可以点击 Code 然后调用 Github Desktop 直接 clone 项目
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023010229811.png" alt="image-20211023005301191" style="zoom:50%;" />





## Idea With Git

> Github Desktop 虽然好用，但我们更多的用的是 idea 里的窗口化

### idea有关Git的基本设置

1、安装 Git

> idea 必须安装 git 才能使用 git 窗口化<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoratyporaimage-20211022221020408.png" alt="image-20211022220705131" style="zoom: 33%;" />
>
> 下载地址（注意有强，自己解决）：https://git-scm.com/download/win

2、在经历了上面的  Github Desktop 给 Test 项目创建仓库后，idea 会出现下图标志

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023001120982.png" alt="image-20211022223113119" style="zoom:50%;" />

3、在 idea 中登录 github 账号，打开设置

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022221827273.png" alt="image-20211022221827273" style="zoom: 40%;" />

4、注意，这里选择 Token 登录

> 用 Token 不直接用  Github 账号登是因为我一直没有用账号登起过，如何拿到 Token 请往下看

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022221928674.png" alt="image-20211023001120982" style="zoom:50%;" />

5、进入你的 Github 网页，点击右上角头像，在点击 Settings

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022222239011.png" alt="image-20211022221928674" style="zoom: 50%;" />

6、点击左边栏下面的 Developer settings

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022222420637.png" alt="image-20211022222239011" style="zoom:50%;" />

7、点击  Personal access tokens，在点  Generate new token

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022222612293.png" alt="image-20211022222612293" style="zoom:40%;" />

8、设置名称、过期日期，再把**所有的都✔**

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022223004291.png" alt="image-20211022225956470" style="zoom:50%;" />

9、生成后点击下图的复制图标

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022223113119.png" alt="image-20211022224327576" style="zoom:67%;" />

10、回到第 4 步，粘贴 Token，完成登录

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022223201057.png" alt="image-20211022222420637" style="zoom:50%;" />





### 新建一个类再push到云端

1、如果我在 src 文件夹下新建了一个类，则会弹出下图

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022223543205.png" alt="image-20211022223004291" style="zoom:50%;" />

> 这个意思是是否直接使用 add 指令，学过 git 指令应该都知道选择什么，如果不知道，**请先学习 git 指令**

2、选择了 Add 后，可以发现类名变绿了

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022224327576.png" alt="image-20211022223201057" style="zoom:50%;" />

> 变绿即代表已对该类使用过 add 指令

3、这里我简单的就只写个 main 函数，请记住下图左边栏的颜色（现在没有任何其他颜色）

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022224522086.png" alt="image-20211022223543205" style="zoom:50%;" />

4、点击前面提到的 commit

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022224711484.png" alt="image-20211022224711484" style="zoom:50%;" />

5、在弹出来的左边窗口中写个简单的描述，再点击  commit

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022225036691.png" alt="image-20211022230638721" style="zoom: 50%;" />

> 在这里简单写的 commit，可是有一定规范的，请[点我](#Commit 规范)

> 图中在描述上方有一个 Amend 按钮，该按钮较常用，教程请[点我](#Amend 按钮)
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022225413728.png" alt="image-20211022224522086" style="zoom:50%;" />
>
> **注意：这里可不要点！**

6、commit 后可发现类名不再是绿色了，此时我们可以 push 代码到远端，点击如图按钮

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022225956470.png" alt="image-20211022225036691" style="zoom:50%;" />

> 然后出现下图界面，这界面相信大家都看得懂，一般情况下直接点击 Push 即可
>
> 1、该界面可以选择 Push 到的远端分支，点击修改 origin : main 即可实现
>
> 2、还可实现强制退送到云端，选择 Push 按钮右边的箭头可改为强推，具体的请看[回退后的 Push](#回退后的 Push)
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022230106611.png" alt="image-20211022230459658" style="zoom:50%;" />

7.1、如果右下角出现该图，很不幸，就算你翻了强也会出现，我怀疑这是 idea 里的 github 插件问题，跟登录要用 Token 一样

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022230459658.png" alt="image-20211022225413728" style="zoom:38%;" />

> 那该怎么办呢？
>
> 这就是我要用 Github Desktop 的原因了，打开 Github Desktop，可以看到左下角已经有了一次 commit
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022230638721.png" alt="image-20211022230749373" style="zoom:33%;" />
>
> 直接点击右上角的<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoratyporaimage-20211022230749373.png" alt="image-20211022230106611" style="zoom:50%;" />
>
> Github Desktop 在番强的情况下，几乎都能成功

7.2、不管你是用 idea 还是 Github Desktop 上传成功，该步直接打开你的 github 网页（之前提到过 Github Desktop 有快捷打开方式）

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022231509784.png" alt="image-20211022232322091" style="zoom:50%;" />





### 修改代码再push

1、开始修改代码

> - 增加代码会出现下图的绿色颜色显示，它是会与你上次 commit 的对应位置进行智能判断的
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022232227572.png" alt="image-20211022232726511" style="zoom:50%;" />
>
>
>
> - 删除代码会像下图显示并且那个箭头支持点击，里面有撤销的功能
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022232322091.png" alt="image-20211022231509784" style="zoom:50%;" />
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022232435976.png" alt="image-20211022232227572" style="zoom:50%;" />
>
>
>
> - 修改之前的代码会出现蓝色显示
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211022232726511.png" alt="image-20211023001212608" style="zoom:50%;" />

2、接下来就是重复之前的 commit 和 push 操作，看之前的 4 — 7.2





### 如何回退到之前commit的代码

> **以下为高阶操作，请在熟悉前面的操作下再看**
>
> 如果不小心 commit 错了，想回退到之前的 commit 怎么办？接下来由 commit 的情况是否已经 push 到云端来分情况讨论
>
> 我先倒着讲回退后要处理的麻烦事

#### 回退后的Push

1、已经 push 到云端

> 这里的已经 push 到云端是指如下情况：
>
> 本地有三次提交分别为：A - B - C，此时云端有也 A - B - C，可我发现 B、C 的提交都有问题，必须回到 A 的基础进行修改（简单来说就是回退到 A，但要删除的 B 和 C 都在云端存在）
>
> 好，那么我们先在本地（idea中）回退到 A 的代码，该好后生成了一个新的提交 D **在本地**
>
> 那么本地的 commit 变为 A - D
>
> 此时就会出现与云端 commit 不同的情况，那么我想删除掉云端的 B 和 C 怎么办？这里只有强推到 github 了（在 idea 中的强推操作看之前的第 6 步）
>
> **注意：**如果该项目是多人开发项目，强推为**危险**操作！！！因为可能别人已经 pull 了 B 和 C 的 commit，你的强推会删除 B 和 C，导致别人的 commit 无法提交到云端，所以在这种情况下，请与整个项目团队进行沟通（提交不规范，辞职两行泪）

2、没有 push 到云端

> 这里的没有 push 到云端指下面的情况：
>
> 本地有三次提交分别为：A - B - C，此时云端只有 A ，我发现B、C 的提交有问题，必须回到 A 的基础进行修改（简单来说就是回退到 A，但要删除的 B 和 C 都在云端不存在）
>
> 万幸你是这种情况，你只需要在本地回退即可

#### 如何在本地回退

> 了解了回退后会出现的问题，你应该知道了一般是不要回退的

1、点击历史<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoratyporaimage-20211023001212608.png" alt="image-20211022232435976" style="zoom:50%;" />

2、选择 Log 窗口

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023005033760.png" alt="image-20211023002718587" style="zoom:50%;" />

3、在你想要回退到的 commit 右键

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023004416934.png" alt="image-20211023005033760" style="zoom:50%;" />

4、弹出来一个窗口，如果是想彻底删除 B 和 C 的 commit，就选 Hard，其他几个可以自己网上百度区别

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023005428419.png" alt="image-20211023004416934" style="zoom:50%;" />

5、Ok，你接下来就会看到少了一个 commit，所以回退请一定要想好后才使用

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023005656460.png" alt="image-20211023005656460" style="zoom:50%;" />





### 分支操作

> **分支为后期必学的操作**
>
> idea 里面提供了分支的快捷操作
>
> 分支一般用于较大型的项目中，用于在某次提交后切一个分支快速修改 bug，或者多人开发中切一个分支用于自己开发新的需求，到 bug 修完或者需求开发完后 git 可以智能的与最新分支进行合并

### 新建分支

1、idea 右下角可以看到目前你所处的分支

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023104427352.png" alt="image-20211023104427352" style="zoom:50%;" />

> 可看到目前我所处 main 分支中
>
> 可能有些人是 master 分支，这时因为 Github Desktop 创建仓库默认 main 为主分支，而 git 默认 master 为主分支
>
> 为方便，后面我以 main 为主分支进行操作

2、点击 main 后可以看到本地所有分支和云端所有分支

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023104819047.png" alt="image-20211023104819047" style="zoom:50%;" />

> 这里本地和云端只有 main 分支，给你们看看网校一项目的分支
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023105250336.png" alt="image-20211023105250336" style="zoom:50%;" />
>
> 可看到云端分支有一大堆，本地分支只有我需要涉及的需求或者 bugfix 分支

3、接下来我们点击 New Brance，创建属于自己的开发分支

> **注意：**新建分支前如果有未 commit 而修改的代码，请把当前所在的分支 commit 一下，不然在新分支的 commit 后，当前分支没有 commit 时做的代码修改将会全部丢失（来自我含泪白写一堆代码后的教训 :(  ），所以如果有未 commit 而修改的代码**一定要 commit 后新建分支或者 Checkout 分支**

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023105903156.png" alt="image-20211023105903156" style="zoom:50%;" />

> - 分支规范如上图，名字 / 类型 / 干什么
    >
    >   如果该项目只有一个人，可以自己放飞自我，写个 dev 就行，但多人开发中可不建议直接这样
>
> - 其中分支名用 “/” 斜杠，会创建分支文件夹，且一创建就直接进入了该分支
>
> - 刚创建后的新分支与 main 分支相同，拥有刚创建时 main 的所有 commit
>
> ![image-20211023110530332](https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023110530332.png)

4、新分支操作与 main 分支相同，我们先修改新分支下的代码，在新分支中 commit 一下

> - 其中，我写了一个 test 方法
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023111042218.png" alt="image-20211023111042218" style="zoom:50%;" />
>
> - 然后再 commit 一下
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023111222995.png" alt="image-20211023111222995" style="zoom:50%;" />
>
> - 然后打开 Git 窗口
    >
    >   <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023111320858.png" alt="image-20211023111320858" style="zoom: 50%;" />
    >
    >   ==================================================================================
    >
    >   <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023111458829.png" alt="image-20211023111458829" style="zoom:50%;" />
    >
    >   > 这里我们可以发现 Git_tutorial 分支比 main 分支多了一次 commit

5、新的 commit 已经生成了，我们如何将新分支提交到云端？

> - 操作与 main 分支相同，直接点击 push 即可
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023111736292.png" alt="image-20211023111736292" style="zoom:50%;" />
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023111857715.png" alt="image-20211023111857715" style="zoom:50%;" />
>
> - push 成功后，打开 Github 网页，其中 Compare & pull request 是云端合并分支
    >
    >   <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023112411362.png" alt="image-20211023112411362" style="zoom:50%;" />

6、本地 main 分支合并新分支的代码

> Compare & pull request 是云端合并分支，但目前新分支与 main 分支都在我本地，没有必要在云端合并

> - 合并前，先切回到被合并的 main 分支
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023113149792.png" alt="image-20211023113149792" style="zoom:50%;" />
>
> - 将新分支的代码合并进 main 分支
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023113657607.png" alt="image-20211023113657607" style="zoom:50%;" />
>
> - 合并后，再打开 Git 窗口，现在 main 分支已经有新分支的提交了，且代码也与新分支相同
    >
    >   ![image-20211023114047791](https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023114047791.png)
>
> - 接下来就可以直接将 main 分支 push 到云端
    >
    >   <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023114618906.png" alt="image-20211023114618906" style="zoom:50%;" />



### 删除分支

> - 确保分支不需要后就可以删除，删除很简单，以下是本地分支的删除
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023114823021.png" alt="image-20211023114823021" style="zoom:50%;" />
>
> - 本地分支虽然被删了，但还有云端分支，操作是一样的，点击 Remote Branches 里的分支删除即可

    >  **但**，这里我保留云端分支额外讲一下：本地无分支，如何切到云端分支？
>
> > 在此之前，请记住之前我含泪重写的教训，**如果当前分支有未 commit 的改动，请先 commit！**
>
> - 切换云端分支其实很简单，点击想切的云端分支，再 Checkout 即可
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023120306069.png" alt="image-20211023120306069" style="zoom:50%;" />
>
> - 我们可以发现 idea 会自动下载云端分支到本地
    >
    >   <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023120422620.png" alt="image-20211023120422620" style="zoom:50%;" />



### 从云端更新分支并合并分支

> **如果你看到了这里，那你简单的分支操作应该会用了，接下来是多人开发时 Git 的使用，可以在用到时再来看**
>
> 这里只讲多人开发中项目级的分支操作，对于两个人同时修改一个分支之后有时间再写 :)
>
> 你说为什么会从云端更新分支呢？
>
> 其实是多人开发中就会出现这种情况
>
> 在多人开发中我们一般有多个分支，比如有一个 master 分支用于主分支，其余的是团队中每个人用于开发需求或者修改 bug 的分支，这些分支在完成后都会提一个 Compare & pull request 在云端与 master 合并分支
>
> （注：开发者不应该拥有对 master 分支的修改权限，一般我们是还有一个 develop 分支，我们将自己的分支与 develop 进行在云端合并，然后交给项目负责人来合并 develop 和 master 分支。develop 分支也不是用于我们开发的，只用于**在云端**合并我们自己的分支，且 develop 分支对于我们本地操作来说只有更新时 pull 下来，再与自己的分支合并的操作）
>
> 为方便，我以网校一项目为例

1、develop 分支在云端已经有了新版本

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023122058529.png" alt="image-20211023122058529" style="zoom:50%;" />

2、将新的 develop 分支与自己的分支合并

> **请注意该点！！！**
>
> **一定要注意！！!**
>
> 如果你的分支有未 commit 的大改动，在合并前**一定要先**在自己的分支**进行一次 commit！！！**，再与 develop 分支合并，来自多位学长泪的教训
>
> 原因在于你也不知道有没有其他人改了你的代码（在项目耦合度高时，极其容易发生），如果你不 commit 直接合并，那么你的代码极可能直接被他人的覆盖。
>
> 如果我提醒了你，你还出现了这种情况，那就 Ctrl + Z 回退吧（如果合并时生成了新的提交，回退大法也救不了你，只能自己靠记忆改回去了:(  ）

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023123258299.png" alt="image-20211023123258299" style="zoom:50%;" />





### 分支操作注意事项！！！

1、**切换分支**或者 new 一个新分支前，如果有未 commit 的代码，**请一定要 commit！！！**

2、合并分支前，**请一定要 commit！！！**



## 最后

> 我一般喜欢用 Github Desktop 创建本地仓库，然后 idea 进行 commit、push、pull 操作，如果 idea 的 push 出现玄学问题。就直接用 Github Desktop 进行 push
>
> 基本的 Git 操作就讲完了，到后面你们还会学习多人开始时 Git 操作，到时候会再进行讲解

## 结语

> 窗口化虽然可以方便操作，但命令行是基础，还是有必要掌握的
>
> 其实 Git 我也只是会一些基本操作，如果教程中有错误的地方请帮我指出一下，感谢！
>
> 作者：郭祥瑞
>
> 最后修改时间：21-10-23，13：00

# 补充

## git学习推荐网站

1、首推：[廖老师的官网](https://www.liaoxuefeng.com/wiki/896043488029600)（别想错了，不是我们的廖老师，但我们的廖老师更强[狗头]）

2、视图化的学习 git：[Learn Git Braancing](https://learngitbranching.js.org/?locale=zh_CN)（一个用视图化学习 git 分支操作的网站）

## 改host访问Github

1、[点我看教程](https://zhuanlan.zhihu.com/p/368485412#:~:text=%20%E5%BE%88%E5%A4%9A%E4%BA%BA%E4%BC%9A%E5%87%BA%E7%8E%B0%EE%80%80Github%EE%80%81%E7%AA%81%E7%84%B6%EE%80%80%E7%99%BB%E4%B8%8D%EE%80%81%E4%B8%8A%E5%8E%BB%EF%BC%8C%E6%88%96%E8%80%85%E8%AE%BF%E9%97%AE%E9%80%9F%E5%BA%A6%E5%BE%88%E6%85%A2%E7%9A%84%E9%97%AE%E9%A2%98%E3%80%82%E5%85%B6%E5%AE%9E%E6%94%B9%E4%B8%AAHOST%E5%B0%B1%E8%83%BD%E8%A7%A3%E5%86%B3%E3%80%82%20%E6%89%BE%E5%88%B0%E4%BC%98%E7%A7%80%E7%9A%84%E8%AE%BF%E9%97%AE%E5%BB%B6%E8%BF%9FIP,%E6%88%91%E4%BB%AC%E5%8E%BB%20%E7%BD%91%E7%AB%99%E6%B5%8B%E9%80%9F%20%E6%B5%8B%E8%AF%95%E5%85%A8%E7%90%83%E5%90%84%E5%9C%B0%E8%BF%9E%E6%8E%A5%EE%80%80github%EE%80%81.com%E7%9A%84%E6%9C%8D%E5%8A%A1%E5%99%A8IP%E5%92%8C%E5%93%8D%E5%BA%94%E9%80%9F%E5%BA%A6%EF%BC%8C%E9%9C%80%E8%A6%81%E4%B8%80%E6%AE%B5%E6%97%B6%E9%97%B4%E6%B5%8B%E8%AF%95%E5%85%A8%E9%83%A8%E6%95%B0%E6%8D%AE%E3%80%82)

2、打开 cmd 输入 ipconfig/flushdns

> 不会改  host
>
> --->[**请百度**](https://baidu.com)
>
> 不会 cmd
>
> --->[**请百度**](https://baidu.com)

3、改 host 仍然会存在不稳定的情况，这个就要靠你们自己解决了

## Amend按钮（改正上一次提交）

> 该按钮用于以下情况：
>
> 比如我上一秒 commit 了代码（**注意：前提是我还没有提交代码到远端**），可下一秒突然发现一个 bug，改完后此时就出现这样的需求：我秀这个 bug 写的代码很少，我不想生成一次新的提交，此时就可以用到这个 Amend 按钮用于合并到上次提交
>
> 请一定要**注意前提**：**我还没有把这次 commit 提交到云端**，如果你已经提交了，就老老实实的生成一次新的提交吧，如果你在这种情况下使用该按钮，会造成本地提交与云端提交不一致，这时你只能自己回退代码了

1、比如我写了个 amen 方法（本来要写 amend）

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023002237750.png" alt="image-20211023002237750" style="zoom:40%;" />

2、结果我没注意，直接生成 commit 了（本来我要写的是 amend() 方法，少了一个字母 d）

<img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023002718587.png" alt="image-20211023005428419" style="zoom:50%;" />

3、在**还没有提交到云端前**我发现了这个问题，这时我不想生成一次新的 commit 来修护这个问题，就可以用 Amend() 来合并到上次提交

> 先修改至正确的代码
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023003142321.png" alt="image-20211023003142321" style="zoom:50%;" />
>
> 然后再提交中，选上 Amend 按钮，可以发现注释直接变成上一次的，在这里可以修改上一次的描述
>
> <img src="https://img-1307243988.cos.ap-chengdu.myqcloud.com/typora/typoraimage-20211023003613262.png" alt="image-20211023003613262" style="zoom:50%;" />

4、最后再说一遍，前提是**这次提交还没有 push 到云端**，出问题了自己去回退 commit 解决

## Commit规范

> 描述写法如下：
>
> ```
> [type]title
> describtion
> ```
>
> type如下：
>
> - fix -------------> bug 修护
> - feature -------> 需求
> - optimize ------> 优化
> - release --------> 版本升级
> - style ------------> 代码格式调整，不涉及代码更改
>
> title：需求标题（对于该commit的简单描述）
>
> describtion：需求的具体描述（如果过于简单的提交可以不用写该部分）
>
> 若提交消息有说明遗漏，可以通过 [Amend](#Amend 按钮) 进行补救
>
> 教程的图中已有演示x

## License
```
Copyright 2022 郭祥瑞

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

