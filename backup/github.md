# git使用

## 英文

### 1-1github里
**issue**  问题，任务，议题   
​	示例：`Submit an issue to report a bug`（提交一个问题报告 Bug）。

------
**Repositories**：简称 **Repo**      代码仓库 或 项目仓库 
**Fork** ：派生 / 复刻  复制他人的仓库到自己的账户，便于修改和开发。
 **Pull Request (PR)** : 拉取请求  向原始仓库提交代码更改请求，用于代码审查和合并。示例：`Open a pull request`（创建一个拉取请求）。

------
**Clone - 克隆** 将远程仓库复制到本地，方便在本地开发。示例：`Clone the repository using HTTPS or SSH`（使用 HTTPS 或 SSH 克隆仓库）。
**Commit - 提交**  将代码修改记录保存到仓库中。  示例：`Make a commit with a clear message`（提交时写明清晰的信息）
**Branch - 分支**   用于开发新功能或修复 Bug，不影响主分支（main/master）。示例：`Create a new branch for the feature`（为这个功能创建一个新分支）。
**Merge - 合并**  将分支的更改合并到主分支或其他分支中。将分支的更改合并到主分支或其他分支中。
**Main/Master - 主分支**  仓库的默认分支，通常存放稳定版本的代码。示例：`Push changes to the main branch`（将更改推送到主分支）。
**Tag - 标签**  标记特定版本，通常用于发布新版本。- 示例：`Create a tag for the new release`（为新版本创建一个标签）。
 **Action - 动作**  GitHub Actions 是一种自动化工具，用于 CI/CD 流水线。示例：`Configure GitHub Actions for testing`（为测试配置 GitHub Actions）。
**Release - 发布** 创建一个特定版本的发布版本，通常包含二进制文件和更新说明。示例：`Download the latest release`（下载最新版本）。
**README - 自述文件**  仓库的首页文件，通常是 `README.md`，包含项目介绍和使用说明。示例：`Update the README file with new information`（更新自述文件的信息）。
**Star - 星标 ** 表示对项目的喜欢或关注，相当于点赞。
**Watch - 关注 ** 订阅仓库更新，收到更新通知。
**Contributor - 贡献者**
**License - 许可证**  项目的开源许可证，规定了使用和修改的权限。示例：`This project is licensed under MIT License`（该项目使用 MIT 许可证）。
**Push - 推送**  将本地的提交推送到远程仓库。
**Pull - 拉取**  从远程仓库拉取最新的更改到本地。

---

---

---

---

### 其他

**订阅（Subscribe）**
**dev**		1、development开发
		       2、linux中 decice（设备）  /dev 是一个特殊的目录，存放所有设备文件 

**lib** library(库文件)，目录或文件夹，存放程序库文件，库文件包含程序运行所需的共享代码，函数资源



**Submit New Issue**  

- 在 GitHub 中，**"Submit New Issue"** 的中文翻译是 **"提交新问题"** 或 **"创建新议题"**。这是你完成 Issue 填写后，用于最终提交 Issue 的按钮。





## GitHub Actions 和Deploy from a Branch

![image-20241111200357355](C:\Users\13729\AppData\Roaming\Typora\typora-user-images\image-20241111200357355.png)

### **1. GitHub Actions**
- **推荐使用场景**：如果你使用了框架（例如 Jekyll、Hugo、Next.js、React 等），并且需要自定义构建流程时，GitHub Actions 是最佳选择。
- **工作原理**：GitHub Actions 是一种 CI/CD（持续集成/持续部署）工具，它可以自动化执行一系列任务，例如安装依赖、构建项目、测试和部署。
- 优势

  - 可以定制化构建流程。
  - 支持复杂项目（例如，使用 JavaScript 框架的项目）的部署。
  - 自动化部署，节省手动操作的时间。
  
- **适合用户**：适合有复杂构建需求的用户，或者希望自动化整个发布流程的用户。

### **2. Deploy from a Branch**
- **推荐使用场景**：如果你的项目是一个简单的静态网站（HTML、CSS、JavaScript 文件），或者使用 GitHub Pages 的经典方式部署，选择这个选项会更简单。
- **工作原理**：你可以选择某个分支（如 `main`、`gh-pages`），GitHub Pages 会直接从该分支读取内容并部署网站。
- 优势

  ：

  - 简单快捷，适合不需要额外构建的静态页面。
  - 配置更简单，适合不需要自定义构建流程的项目。

- **适合用户**：适合构建需求简单的用户，特别是静态网站或个人博客用户。
### **总结**
- **GitHub Actions**：适合复杂项目，需要自定义构建和自动化部署。
- **Deploy from a Branch**：适合简单项目，直接从分支发布网站。
### **如何选择**
- 如果你的项目使用了现代 JavaScript 框架或构建工具（如 `npm`、`webpack`），推荐使用 **GitHub Actions**。
- 如果你只是发布一个简单的 HTML 网站，选择 **Deploy from a Branch** 更为方便。

# lesson

## git 与github基础介绍

**基础介绍**

- 账号
- 双重身份验证
- 仓库功能
- READNE/issue/release/PR （pull request）
- github快捷键

---

---



### **git使用**

git 用于版本控制的软件
git 使用commit(提交)作为版本控制的基本单元————————理解成历史记录，每次改动都会被commit链路记录下来

#### 	2-3-1 git命令行

- git bash
  bash就是linux和mac系统的命令行工具，后来被移植到Windows上。————git bush
  cmd是Windows自带的命令行工具	<img src="D:\博客图片暂存\Screenshot_20241112_092738.jpg" style="zoom:50%;" />注意：rm -rf /切勿在linux中尝试！删除电脑中全部文件

  实践1：![image-20241112095354951](D:\博客图片暂存\image-20241112095354951.png)

​	实践发现：

- cd ..  中间有空格
- rm -r  有空格

Windows下清屏是cls
快捷方式文件（.lnk 后缀）

---

**gitbash**

- 在gitbash里执行cd /在使用ls列出根目录，显示的是git的安装目录中的文件和文件夹
​	在gitbash中，/不是指windows系统的根目录，而是gitbash的虚拟根目录（git安装目录）
​	切换到C盘：  cd /c/

- ~是指用户主目录

  cd ~        会带到       C：\users\13729

  echo ~    查看主目录路径  C：\users\13729

​	

---

#### 	2-3-2 git配置

- 所有的配置文件其实都保存在本地

---

git config -l  (l就是list)
git config --system --list 查看系统配置
git config --globlal --list   (global就是全局) 看本地：用户自己配的：用户名和密码

![image-20241112105336346](D:\博客图片暂存\image-20241112105336346.png)



---

- git的安装目录

<img src="D:\博客图片暂存\屏幕截图 2024-11-12 111301.png" style="zoom: 67%;" />









##### 仓库

- Local Repository 
- Remote Repository -----github

#####  github快捷键

1.  /  快速搜索
2.  L  快速定位行号
3. T  定位到文件搜索栏
4. ![image-20241111191616315](C:\Users\13729\AppData\Roaming\Typora\typora-user-images\image-20241111191616315.png)

![image-20241111191718218](C:\Users\13729\AppData\Roaming\Typora\typora-user-images\image-20241111191718218.png)

输入？————可打开快捷键速查表

5、输入句号。   ————可以申请远程的运行环境，可以直接在浏览器内调试修改代码
GitHub codespace有一定的免费使用额度

![image-20241111192329693](C:\Users\13729\AppData\Roaming\Typora\typora-user-images\image-20241111192329693.png)

### 发现

- GitHub高级搜索功能
- 如何下载运行GitHub开源项目

#### (1)页面1  github.com/explore

![image-20241111192758593](C:\Users\13729\AppData\Roaming\Typora\typora-user-images\image-20241111192758593.png)

#### （2）页面2： https://github.com/search



## github基础操作（网站）

### 3、装修个人主页

- markdown语法

### 4、创建个人仓库

- 选择开源许可证
- commit

### 5、Branch分支

- 修改Branch
- Pull request

### 6、github是如何工作的

### 7、仓库其他功能

- github wiki
- github insight
  - 社区规则
  - 项目统计
  - 安全机器人

- github project
  - github项目管理功能
- github discussions
  - 论坛功能



## Github Desktop

### 8、Github Desktop安装配置

- .git 文件夹到底是什么

### 9、Git四个分区的概念

- 实践git基本操作流程

### 10、desktop进阶操作

- stash
- git后悔药
  - reset
  - discard
  - revert
  - amend
- tag

### 11、分支合并

- merge
- rebase
- squash merge
- cherry pick

### 12、解决合并冲突

### 13、如何给一个开源项目贡献自己的代码



## IDE 使用git





## git命令行操作





## github action



## github pages

## 项目

​                                 







###  博客

- **手动构建**

![image-20241111214839589](C:\Users\13729\AppData\Roaming\Typora\typora-user-images\image-20241111214839589.png)



# 其他问题

1. 下载太慢————拉镜像

2. - - 1. 

​			



