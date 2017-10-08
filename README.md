# xnx3_language
Java 多国语言包，极简方式，快速让Java拥有多语言切换能力


## 最简单的，为项目快速创建多种语言支持，只需两步
#### 1. /language.xml 为语言包配置文件，语言都是在这里配置。将其放到src目录下
#### 2. /lib/ 文件夹下为所依赖的jar包，将其导入项目
#### 3. 在项目中调取指定的语言文字显示：
```Java
    Language.show("chinese", "login");
```


### /demo/ 文件夹下为一个提供演示的java project的demo示例