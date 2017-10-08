# xnx3_language
Java 多国语言包，极简方式，快速让Java拥有多语言切换能力
<br/>
<hr/>

## 最简单的，为项目快速创建多种语言支持，只需两步
#### 1. /language.xml 为语言包配置文件，语言都是在这里配置。将其放到src目录下
#### 2. /lib/ 文件夹下为所依赖的jar包，将其导入项目
#### 3. 在项目中调取指定的语言文字显示：
```Java
    Language.show("chinese", "login");
```
#### /demo/ 文件夹下为一个提供演示的java project的demo示例
<br/>
<hr/>

## 在web项目中使用时，使用Cookie＋Session进行存储用户当前选择的语言，下次进入时，直接使用用户自己上次选择好的语言显示出来
#### 在jsp页面上显示指定语言的登录(login)文字
```Java
    LanguageWeb.show(HttpServletRequest, HttpServletResponse, "login");
```
#### 用户自己从页面上选择使用英文来显示，那么将用户选择的语言包存入cookie、session，下次调用show()显示的时候，直接显示用户自己选择的语言
```Java
    LanguageWeb.setCurrentLanguagePackageName(HttpServletRequest, HttpServletResponse, "english");
```
