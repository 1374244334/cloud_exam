## 答题小程序云开发版

使用小程序原生云开发搭建。
界面使用-[ColorUI](https://github.com/weilanwl/ColorUI)

## 目标功能：

1. 由原生云数据库储存题库。

2. 随机出题。

3. 回答评分。

4. 练习题目。

5. 预约教师。
    
## 目前以实现功能：

1. 随机从题库中抽取题目，以及答题页面的实现。

2. 登录界面美化。

3. 评分功能构建，使用云函数。

4. 关于页面构建完成。

5. 教师预约，评分，留言功能。

基本完成全部功能，除了欢迎界面太丑暂时不想更改。

## 部分截图

![稿定设计导出-20210227-105104](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614394310782-%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1%E5%AF%BC%E5%87%BA-20210227-105104.jpg)
![稿定设计导出-20210227-105137](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614394318798-%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1%E5%AF%BC%E5%87%BA-20210227-105137.jpg)


## 部署文档

1. 注册微信小程序账号，直接按照官方文档操作，不做具体演示。

2. 将仓库代码克隆到本地。用微信小程序开发工具打开。

![Snipaste_2021-02-27_10-30-41](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393062426-Snipaste_2021-02-27_10-30-41.png)

3. 设置云开发环境。这里生成的云开发环境中的ID，需要在微信小程序代码中做配置。后面都统一叫做云开发环境ID。

![Snipaste_2021-02-27_10-31-52](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393123166-Snipaste_2021-02-27_10-31-52.png)

4. 配置云开发环境ID。

![Snipaste_2021-02-27_10-33-15](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393238145-Snipaste_2021-02-27_10-33-15.png)

5. 创建集合。点击微信开发者工具栏上的云开发菜单，跳转到云开发控制台。

![Snipaste_2021-02-27_10-35-11](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393376465-Snipaste_2021-02-27_10-35-11.png)
![Snipaste_2021-02-27_10-35-59](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393387943-Snipaste_2021-02-27_10-35-59.png)

> 这里需要特别说明一下，questionBank中的字段，需要自己手动创建。具体的格式参考代码仓库中的exam_demo.json文件。

6. 同步云函数库。用微信开发者工具打开代码，可以看到如下的目录。


![Snipaste_2021-02-27_10-38-29](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393616549-Snipaste_2021-02-27_10-38-29.png)

鼠标选中cloudfunctions目录，右键，选择同步云函数。

![1614393542968](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393671475-1614393542968.jpg)

同步成功之后，云开发控制台中的云函数列表，则有如下几个函数。

![Snipaste_2021-02-27_10-37-57](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393727623-Snipaste_2021-02-27_10-37-57.png)

7. 导入模拟数据。

点击云开发控制台中的数据库，接着选中questionBank集合，选择导入按钮，选中代码仓库中的exam_demo.json文件。

![Snipaste_2021-02-27_10-42-51](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393848742-Snipaste_2021-02-27_10-42-51.png)

## 问题

使用中有什么问题，可以咨询与反馈。

![WechatIMG39](https://gitee.com/bruce_qiq/picture/raw/master/2021-2-27/1614393893107-WechatIMG39.jpeg)




