# Maven

### 1.传递依赖重复

引入了2个项目，两个项目里均引入了相同的jar，需要排除一个，避免产生冲突。

### 2.寻找重复包的传递依赖的方式
- **用命令**	
	- mvn install 打包
	- mvn dependency:tree 查看传递依赖树
- **插件查看**
	- 安装插件maven helper
	- 打开项目的pom文件

### 3.排掉传递依赖后重复的jar
```
  <exclusion>
                       
  </exclusion>

```