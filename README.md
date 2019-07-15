# test-sys-server
# 考试系统后端

>这是一个考试系统的后端，前端的仓库还没搭建，（这个项目也不知道什么时候能完成），后端按照目前的想法，后端支持2种运行模式。

### 数据库模式

在这个模式下，通过本地的配置文件，访问服务器。前端发送用户登录的数据过来，登录通过并且前端点击开始考试，那么将考试题目发送到前端，当考试结束用户点击提交后，后端就会向前端发送题目答案，前端把选择填空题的成绩计算出来，然后把成绩和主观题的数据发送到后端，并存入数据库。

数据库使用mysql和Redis，mysql主要用于存储用户的信息，Redis用于考试时存放考题。

### 文件模式

这个模式也是跟数据库模式类似，就是把数据库的内容全部放到文件里面，运行模式也是一样。



---
2019-1-15
