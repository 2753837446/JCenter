# JCenter

### 此项目适用于所有想要上传自己的Library到Jcenter的程序猿们
### 1.配置
> 配置方法如下参见项目中的 
> https://github.com/2753837446/JCenter/blob/master/build.gradle
> https://github.com/2753837446/JCenter/blob/master/library/build.gradle
> 项目根目录下的installv1.gradle, bintrayv1.gradle 是必须要添加的, 不可修改, 如果路径有修改, 对应的修改module中的配置

### 2.账号配置
>在项目的local.properties文件中添加在JForg Bintray中创建的用户名和key
>bintray.user=xxxx
>bintray.apikey=xxx

### 3.开始上传
>命令行运行到对应的Module下 
>./gradlew install   出现 BUILD SUCCESS就ok
>./gradlew bintrayUpload  出现 BUILD SUCCESS后就可以去Bintary后台看一下是否添加成功, 如果进入maven后发现其中多了一个package 那就是成功了
