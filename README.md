> #### 作者主页：[舒克日记](https://blog.csdn.net/cativen)
>
>  简介：Java领域优质创作者、Java项目、学习资料、技术互助
>
> <b><font color=red>文中获取源码</font></b>

# 项目介绍

高校学生管理系统有管理员，教师，学生三个角色。

​

有个人中心，教师管理，学生管理，学生请假管理，课表信息管理，院系班级管理，学生奖惩管理，学生成绩管理，培养计划管理，课程信息管理。教师和学生都可以注册登录。

教师主要对学生请假信息进行审核，对其他信息进行管理。

# 环境要求

1.运行环境：最好是java jdk1.8,我们在这个平台上运行的。其他版本理论上也可以。

2.IDE环境：IDEA,Eclipse,Myeclipse都可以。推荐IDEA;

3.tomcat环境：Tomcat7.x,8.X,9.x版本均可

4.硬件环境：windows7/8/10 4G内存以上；或者Mac OS;

5.是否Maven项目：是；查看源码目录中是否包含pom.xml;若包含，则为maven项目，否则为非maven.项目

6.数据库：MySql5.7/8.0等版本均可；

# 技术栈

运行环境：jdk8 + tomcat9 + mysql5.7 + windows10

服务端技术：Java、Spring、SpringMVC、Mybatis，SSM

# 使用说明

1.使用Navicati或者其它工具，在mysql中创建对应sq文件名称的数据库，并导入项目的sql文件；

2.使用IDEA/Eclipse/MyEclipse导入项目，修改配置，运行项目；

3.将项目中config-propertiesi配置文件中的数据库配置改为自己的配置，然后运行；

# 运行指导

idea导入源码空间站顶目教程说明(Vindows版)-ssm篇：

http://mtw.so/5MHvZq

源码地址：[http://www.codegym.top](http://www.codegym.top/)

其它问题请关注公众号：**IT小舟**,关注后发送消息即可，都会给您回复的。若没有及时回复请耐心等待，通常当天会有回复

# 运行截图

## 功能模块截图

![img](https://img-blog.csdnimg.cn/img_convert/24fa876c4d60001defb559fc0cff99b2.png)

#### 页面截图

![Snipaste20240908111639](https://img-blog.csdnimg.cn/img_convert/7f212bdc0d42030c11d5812bb8c7b826.png)

![ssm412高校学生管理系统0](https://img-blog.csdnimg.cn/img_convert/a1333b89872c24b17c864ad0a8ea097e.png)

![ssm412高校学生管理系统1](https://img-blog.csdnimg.cn/img_convert/931e5770d72eabcc3170554ace2f66fd.png)

![ssm412高校学生管理系统2](https://img-blog.csdnimg.cn/img_convert/35fad925a5f689f4702d1bd4fc24eac9.png)

![ssm412高校学生管理系统3](https://img-blog.csdnimg.cn/img_convert/0449edd531144ca92231c034c49ccbbf.png)

![ssm412高校学生管理系统4](https://img-blog.csdnimg.cn/img_convert/4fcec2411a9e5c55d80cea4b8048a689.png)

### 代码

```

        MenuDO menuDO = new MenuDO();
        BeanUtils.copyProperties(dto, menuDO);
        if (menuDO.getId() != null) {
            menuDO.setUpdateBy(1);
            menuDO.setUpdateTime(LocalDateTime.now());
        } else {
            menuDO.setUpdateBy(1);
            menuDO.setCreateBy(1);
            menuDO.setCreateTime(LocalDateTime.now());
            menuDO.setUpdateTime(LocalDateTime.now());
            menuDO.setDataStatus(1);
        }
```
