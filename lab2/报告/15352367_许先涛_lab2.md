嵌入式系统导论实验报告
=
---

|  姓名  |  学号  |  班级  |  电话  |  邮箱  |
| :--: | :--: | :--: | :--: | :--: |
| 许先涛  |15352367|1516|17612034037 |ku8834367@163.com|
---
##1.实验题目
    
##&emsp;DOL开发环境配置
<br/>

##2.实验结果
*  下载相关软件环境
    ![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/P0.png)
<br/><br/><br/>
* 编译systemc，运行configure
    ![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/install.png)

<br/><br/><br/>
* 运行install  
    >![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/make0.png)
    >![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/make1.png)

<br/><br/><br/>
* 修改dol文件中的build_zip.xml文件
![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/build_zip.png)

<br/><br/><br/>
* 编译ant文件
![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/build.png)
<br/><br/><br/>
* 编译第一个example
    >![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/buildex.png)
    >(由于C++版本过高出现错误，检查后发现在新版本中是函数std:gets没有识别出来)
    >![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/wrong.png)
    
<br/><br/><br/>
* 上网查找解决方案如下
![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/solution.png)
<br/><br/><br/>
* 运行后successful
![](https://github.com/XuXianTao/Embedded_lab/raw/master/lab2/%E6%8A%A5%E5%91%8A/build_suc.png)
<br/><br/><br/>
##3.实验心得
&emsp;&emsp;这次实验也是主要照着ppt的提示完成就ok了，遇到的问题也就是最后一步的build由于系统自带gcc版本较高无法识别出systemc库中的std:gets导致的编译失败，所以只要将std::gets给相应注释掉就OK了。
&emsp;&emsp;然后是排版的问题，由于在markdown中并不支持图片的直接修改大小，一般都是用html语句进行兼容执行，同时由于无法通过markdown的修改直接看到所导出的pdf具体排版，所以我也只能随机地导出，结果就是导致了pdf的图片排版很不好，目前还找不到什么方法来有效快捷的让pdf的排版也同时顾及到。