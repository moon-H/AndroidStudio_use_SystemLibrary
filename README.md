# AndroidStudio_use_SystemLibrary


1.在libs文件夹同级的目录下建立一个ext（名称随意，systemlibrary 放在此目录下），将只用于编译的jar包放在此。

2.配置buidle.gradle

 dependencies {
 
    provided files('ext/aaa.jar')
    
}

这样aaa.jar包将会参与编译，但不会被打包进apk。

不明白的可以QQ 307313378
