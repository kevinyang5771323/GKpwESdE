# 前言

随着新冠疫情的蔓延，社区防疫工作变得尤为重要。为了提高社区防疫工作的效率和精度，我们基于SSM（Spring、SpringMVC、MyBatis）框架开发了一套社区防疫管控系统。本文将为您详细介绍该项目的相关内容。

# 内容介绍

本系统主要实现了以下功能：

1. 用户管理：包括管理员、社区居民等角色的注册、登录、权限管理等功能。
2. 健康信息填报：社区居民可以在线填报健康信息，系统自动汇总并生成报表。
3. 防疫知识宣传：管理员可以发布防疫相关知识，提高社区居民的防疫意识。
4. 通知公告：管理员可以发布防疫相关通知，确保信息及时传达给社区居民。
5. 防疫物资管理：管理员可以对防疫物资进行增删改查操作，确保物资合理分配。

# 技术介绍

- 语言：Java
- 使用框架：Spring、SpringMVC、MyBatis
- 前端技术：JS、Vue、CSS3
- 开发工具：IDEA/Eclipse
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven：apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

# 核心代码

以下是系统中用于查询社区居民健康信息的核心代码：

```java
// HealthInfoMapper.java
public interface HealthInfoMapper {
    @Select("SELECT * FROM health_info WHERE user_id = #{userId}")
    HealthInfo selectHealthInfoByUserId(@Param("userId") int userId);
}
```

```xml
<!-- healthInfoMapper.xml -->
<mapper namespace="com.example.mapper.HealthInfoMapper">
    <select id="selectHealthInfoByUserId" resultType="com.example.entity.HealthInfo">
        SELECT * FROM health_info WHERE user_id = #{userId}
    </select>
</mapper>
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/286556/14/12748/215523/68b17c02F040d184a/b639dc5689d886b7.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/337471/16/3530/74295/68b17bdaF13dd07d2/e1f2aec13aa0b1cc.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/310128/2/20624/163169/68b17bdaF2150a865/c1692b178b76acc1.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/294832/32/25834/61197/68b17bdbF5fda18c4/2199d0157c6b8fbc.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/326611/40/12813/62531/68b17bdbFd61dd2bb/b7c794158c3e12db.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/339714/4/2941/152749/68b17bdcF3789e262/90dcd5089dbf4204.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/326452/31/12715/52179/68b17bdcFec9982e6/5ad08970ae78cfa9.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/339015/31/3577/85233/68b17bddF7a5f2b3d/c86006b260a95252.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/293284/30/22487/49146/68b17bddF9d388562/77871b89d03d0f14.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/324320/32/12771/68920/68b17bdeF1a509e97/72d0a87b5673e860.jpg)

