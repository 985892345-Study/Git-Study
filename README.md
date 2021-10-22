# 图形化使用 Git 的保姆级教程

## Github Desktop

> 由于很多学弟刚开始学习命令行有些难度，所以这里对 github 的图形化操作进行讲解。
>
> 图形化虽然简单，但命令行也是非常重要的，强烈建议各位学习一下命令行的使用
>
> 注：本教程需要一定 git 基础，且教程内不会教什么是 commit、add、push 等作用，这些请自己学习 git 指令
>
> 还没学习 git 指令的请[点我](#git 学习推荐网站)

> 你说 idea 可以 Github Desktop 的所有操作，为什么还要 Github Desktop？
>
> 因为 idea 里的 GitHub 经常有一些玄学问题，看到后面我会介绍，Github Deskt

### 下载

> 建议使用 edge 或者 Google Chrome

百度搜索 Github Desktop 或者点击 https://desktop.github.com/ 进行下载

### 登录

1、点击Sign in 打开浏览器登录

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211020192222298.png" alt="image-20211020194102498" style="zoom:40%;" />

2、登陆后这里建议更换邮箱为自己注册 github 时的邮箱(点击右边向下箭头)

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211020193744614.png" alt="image-20211020193744614" style="zoom:50%;" />

3、进入这个界面就🆗了

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211020194102498.png" alt="image-20211020192222298" style="zoom:33%;" />

### 创建本地仓库

1、点击左上角 File - Add local repository

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211020194311766.png" alt="image-20211020194311766" style="zoom:50%;" />

> 学长，创建本地仓库为什么不点第一个 New repository?
>
> 其实点第一个也行，但有些坑，第一个更偏向用于创建一个只带有.git文件的空的文件夹，如果想用它来指向你的项目文件夹，需要你手动输入项目文件夹的全名。而第二个就可以直接省去这些步骤。

2、点击 Choose 然后选择你的项目文件夹

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211020195540651.png" alt="image-20211020195540651" style="zoom:50%;" />

> 例如我有一个叫 Test 的项目，就选择他就 OK（别选到里面的 src 这些，我们需要的是整个项目文件）
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211020195416879.png" alt="image-20211020195416879" style="zoom: 50%;" />

3、然后点击 create a repository 创建本地仓库

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211020202240883.png" alt="image-20211020202240883" style="zoom:50%;" />

4、描述和README

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211020203558784.png" alt="image-20211020203558784" style="zoom:50%;" />

5、到这里你的本地仓库就创建完了

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211020200657266.png" alt="image-20211020200657266" style="zoom:50%;" />

> 学长，提交是什么意思？
>
> 提交是 commit，但如果不知道，请先了解 git 指令！

### 创建云端仓库

> 之前我们已经成功创建了本地仓库，接下来将带你创建云端仓库

1、上传本地仓库至 Github，点击下图所示

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023005301191.png" alt="image-20211022214611182" style="zoom: 50%;" />

2、在这里有一个坑，它默认云端仓库是 private，视自己情况可以选择关闭这个选项（但发给我们的作业必须关闭这个）

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022214855455.png" alt="image-20211022214855455" style="zoom:50%;" />

3.1、出现下图一般是墙的问题，这个请看[改host](#改 host 访问 Github)

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023010229811.png" alt="image-20211023005301191" style="zoom:50%;" />

3.2、当左下角的 Initial commit 没有的时候，恭喜你上传成功，接下来点击 View on Github 打开 github（可以记下这个快捷打开方式）

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022221020408.png" alt="image-20211022220705131" style="zoom:50%;" />

4、成功的界面

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022214611182.png" alt="image-20211023005207748" style="zoom:50%;" />

### 更方便的 clone

> 有了 Github Desktop 后，在 github 中可以点击 Code 然后调用 Github Desktop 直接 clone 项目
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022220705131.png" alt="image-20211023010229811" style="zoom:50%;" />

## Idea With Git

> Github Desktop 虽然好用，但我们更多的用的是 idea 里的窗口化

### idea 有关 Git 的基本设置

1、安装 Git

> idea 必须安装 git 才能使用 git 窗口化<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023005207748.png" alt="image-20211022221020408" style="zoom:25%;" />
>
> 下载地址（注意有强，自己解决）：https://git-scm.com/download/win

2、在经历了上面的  Github Desktop 给 Test 项目创建仓库后，idea 会出现下图标志

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022221928674.png" alt="image-20211023001120982" style="zoom:50%;" />

3、在 idea 中登录 github 账号，打开设置

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022221827273.png" alt="image-20211022221827273" style="zoom: 40%;" />

4、注意，这里选择 Token 登录

> 用 Token 不直接用  Github 账号登时因为我一直没有用账号登起过，如何拿到 Token 请往下看

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022222239011.png" alt="image-20211022221928674" style="zoom: 50%;" />

5、进入你的 Github 网页，点击右上角头像，在点击 Settings

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022222420637.png" alt="image-20211022222239011" style="zoom:50%;" />

6、点击左边栏下面的 Developer settings

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022223201057.png" alt="image-20211022222420637" style="zoom:50%;" />

7、点击  Personal access tokens，在点  Generate new token

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022222612293.png" alt="image-20211022222612293" style="zoom:40%;" />

8、设置名称、过期日期，在把**所有的都✔**

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022223543205.png" alt="image-20211022223004291" style="zoom:50%;" />

9、生成后点击下图的复制图标

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023001120982.png" alt="image-20211022223113119" style="zoom:50%;" />

10、回到第 4 步，粘贴 Token，完成登录

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022224327576.png" alt="image-20211022223201057" style="zoom:50%;" />

### 新建一个类再 push 到云端

1、如果我在 src 文件夹下新建了一个类，则会弹出下图

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022224522086.png" alt="image-20211022223543205" style="zoom:50%;" />

> 这个意思是是否直接使用 add 指令，学过 git 指令应该都知道选择什么，如果不知道，**请先学习 git 指令**

2、选择了 Add 后，可以发现类名变绿了

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022223113119.png" alt="image-20211022224327576" style="zoom:67%;" />

> 变绿即代表已对该类使用过 add 指令

3、这里我简单的就只写个 main 函数，请记住下图的颜色

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022225413728.png" alt="image-20211022224522086" style="zoom:50%;" />

4、点击前面提到的 commit

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022224711484.png" alt="image-20211022224711484" style="zoom:50%;" />

5、在弹出来的左边窗口中写个简单的描述，再点击  commit

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022225956470.png" alt="image-20211022225036691" style="zoom:50%;" />

> 图中在描述上方有一个 Amend 按钮，该按钮较常用，教程请[点我](#Amend 按钮)
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022230459658.png" alt="image-20211022225413728" style="zoom:38%;" />

6、commit 后可发现类名不再是绿色了，此时我们可以 push 代码到远端，点击如图按钮<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022223004291.png" alt="image-20211022225956470" style="zoom:50%;" />

> 然后出现下图界面，这界面相信大家都看得懂，一般情况下直接点击 Push 即可
>
> 1、该界面可以选择 Push 到的远端分支，点击修改 origin : main 即可实现
>
> 2、还可实现强制退送到云端，选择 Push 按钮右边的箭头可改为强推，具体的请看[回退后的 Push](#回退后的 Push)
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022230749373.png" alt="image-20211022230106611" style="zoom:50%;" />

7.1、如果右下角出现该图，很不幸，就算你翻了强也会出现，我怀疑这是 idea 里的 github 插件问题，跟登录要用 Token 一样

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022230106611.png" alt="image-20211022230459658" style="zoom:50%;" />

> 那该怎么办呢？
>
> 这就是我要用 Github Desktop 的原因了，打开 Github Desktop，可以看到左下角已经有了一次 commit
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022225036691.png" alt="image-20211022230638721" style="zoom: 50%;" />
>
> 直接点击右上角的 <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022230638721.png" alt="image-20211022230749373" style="zoom:33%;" />
>
> Github Desktop 在范强的情况下，几乎都能成功

7.2、不管你是用 idea 还是 Github Desktop 上传成功，该步直接打开你的 github 网页（之前提到过 Github Desktop 有快捷打开方式）

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022232322091.png" alt="image-20211022231509784" style="zoom:50%;" />

### 修改代码再 push

1、开始修改代码

> 增加代码会出现下图的绿色颜色显示，它是会与你上次 commit 的对应位置进行智能判断的
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022232435976.png" alt="image-20211022232227572" style="zoom:50%;" />
>
> 删除代码会像下图显示并且那个箭头支持点击，里面有回退的功能
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022231509784.png" alt="image-20211022232322091" style="zoom:50%;" />
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023001212608.png" alt="image-20211022232435976" style="zoom:50%;" />
>
> 修改之前的代码会出现蓝色显示
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022232227572.png" alt="image-20211022232726511" style="zoom:50%;" />

2、接下来就是重复之前的 commit 和 push 操作，看之前的 4 — 7.2

## 如何回退到之前 commit 的代码

> **以下为高阶操作，请在熟悉前面的操作下再看**
>
> 如果不小心 commit 错了，想回退到之前的 commit 怎么办？接下来由 commit 的情况是否已经 push 到云端来分情况讨论
>
> 我先倒着讲回退后要处理的麻烦事

### 回退后的 Push

1、已经 push 到云端

> 这里的已经 push 到云端是指如下情况：
>
> 本地有三次提交分别为：A - B - C，此时云端有也 A - B - C，可我发现 C 的提交有问题，必须回到 A 的基础进行修改（简单来说就是回退到 A，但 要删除的 B 和 C 都在云端存在）
>
> 好，那么我们先在本地（idea中）回退到 A 的代码，该好后生成了一个新的提交 D **在本地**
>
> 那么本地的分支变为 A - D
>
> 此时就会出现与云端分支不同的情况，那么我想删除掉云端的 B 和 C 怎么办？这里只有强推到 github 了（在 idea 中的强推操作看之前的第 6 步）
>
> **注意：**如果该项目是多人开发项目，强推为**危险**操作！！！因为可能别人已经 pull 了 B 和 C 分支，你的强推会删除 B 和 C，导致别人的 commit 无法提交到云端，所以在这种情况下，请与整个项目团队进行沟通（提交不规范，辞职两行泪）

2、没有 push 到云端

> 这里的没有 push 到云端指下面的情况：
>
> 本地有三次提交分别为：A - B - C，此时云端只有 A ，我发现 C 的提交有问题，必须回到 A 的基础进行修改（简单来说就是回退到 A，但要删除的 B 和 C 都在云端不存在）
>
> 万幸你是这种情况，你只需要在本地回退即可

### 如何在本地回退

> 了解了回退后会出现的问题，你应该知道了一般是不要回退的

1、点击历史<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211022232726511.png" alt="image-20211023001212608" style="zoom:50%;" />

2、选择 Log 窗口

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023004416934.png" alt="image-20211023005033760" style="zoom:50%;" />

3、再你想要回退到的提交右键

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023005428419.png" alt="image-20211023004416934" style="zoom:50%;" />

4、弹出来一个窗口，如果是想彻底删除 B 和 C 分支，就选 Hard，其他几个可以自己网上百度区别

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023002718587.png" alt="image-20211023005428419" style="zoom:50%;" />

5、Ok，你接下来就会看到少了一个提交，所以回退请一定要想好后才使用

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023005656460.png" alt="image-20211023005656460" style="zoom:50%;" />

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
> 最后修改时间：21-10-23，01：00

# 补充

## git 学习推荐网站

1、首推：[廖老师的官网](https://www.liaoxuefeng.com/wiki/896043488029600)（别想错了，不是我们的廖老师，但我们的廖老师更强[狗头]）

2、视图化的学习 git：[Learn Git Braancing](https://learngitbranching.js.org/?locale=zh_CN)（一个用视图化学习 git 分支操作的网站）

## 改 host 访问 Github

1、[点我看教程](https://zhuanlan.zhihu.com/p/368485412#:~:text=%20%E5%BE%88%E5%A4%9A%E4%BA%BA%E4%BC%9A%E5%87%BA%E7%8E%B0%EE%80%80Github%EE%80%81%E7%AA%81%E7%84%B6%EE%80%80%E7%99%BB%E4%B8%8D%EE%80%81%E4%B8%8A%E5%8E%BB%EF%BC%8C%E6%88%96%E8%80%85%E8%AE%BF%E9%97%AE%E9%80%9F%E5%BA%A6%E5%BE%88%E6%85%A2%E7%9A%84%E9%97%AE%E9%A2%98%E3%80%82%E5%85%B6%E5%AE%9E%E6%94%B9%E4%B8%AAHOST%E5%B0%B1%E8%83%BD%E8%A7%A3%E5%86%B3%E3%80%82%20%E6%89%BE%E5%88%B0%E4%BC%98%E7%A7%80%E7%9A%84%E8%AE%BF%E9%97%AE%E5%BB%B6%E8%BF%9FIP,%E6%88%91%E4%BB%AC%E5%8E%BB%20%E7%BD%91%E7%AB%99%E6%B5%8B%E9%80%9F%20%E6%B5%8B%E8%AF%95%E5%85%A8%E7%90%83%E5%90%84%E5%9C%B0%E8%BF%9E%E6%8E%A5%EE%80%80github%EE%80%81.com%E7%9A%84%E6%9C%8D%E5%8A%A1%E5%99%A8IP%E5%92%8C%E5%93%8D%E5%BA%94%E9%80%9F%E5%BA%A6%EF%BC%8C%E9%9C%80%E8%A6%81%E4%B8%80%E6%AE%B5%E6%97%B6%E9%97%B4%E6%B5%8B%E8%AF%95%E5%85%A8%E9%83%A8%E6%95%B0%E6%8D%AE%E3%80%82)

2、打开 cmd 输入 ipconfig/flushed

> 不会改  host
>
> --->[**请百度**](https://baidu.com)
>
> 不会 cmd
>
> --->[**请百度**](https://baidu.com)

3、改 host 仍然会存在不稳定的情况，这个就要靠你们自己解决了

## Amend 按钮

> 该按钮用于以下情况：
>
> 比如我上一秒 commit 了代码（**注意：前提是我还没有提交代码到远端**），可下一秒突然发现一个 bug，改完后此时就出现这样的需求：我秀这个 bug 写的代码很少，我不想生成一次新的提交，此时就可以用到这个 Amend 按钮用于合并到上次提交
>
> 请一定要**注意前提**：**我还没有把这次 commit 提交到云端**，如果你已经提交了，就老老实实的生成一次新的提交吧，如果你在这种情况下使用该按钮，会造成本地提交与云端提交不一致，这时你只能自己回退代码了

1、比如我写了个 amen 方法（本来要写 amend）

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023002237750.png" alt="image-20211023002237750" style="zoom:40%;" />

2、结果我没注意，直接生成 commit 了（本来我要写的是 amend() 方法，少了一个字母 d）

<img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023005033760.png" alt="image-20211023002718587" style="zoom:50%;" />

3、在**还没有提交到云端前**我发现了这个问题，这时我不想生成一次新的 commit 来修护这个问题，就可以用 Amend() 来合并到上次提交

> 先修改至正确的代码
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023003142321.png" alt="image-20211023003142321" style="zoom:50%;" />
>
> 然后再提交中，选上 Amend 按钮，可以发现注释直接变成上一次的，再这里可以修改上一次的描述
>
> <img src="https://985892345-1307243988.cos.ap-chengdu.myqcloud.com/img/typoraimage-20211023003613262.png" alt="image-20211023003613262" style="zoom:50%;" />

4、最后再说一遍，前提是**这次提交还没有 push 到云端**，出问题了自己去回退 commit 解决



