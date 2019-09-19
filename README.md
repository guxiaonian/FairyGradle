<div align="center">

## FairyGradle

**`gradle`常用工具汇总**

</div>
<br>

# aar文件相关

剔除aar内某个包或个别文件，包名替换

## 使用步骤

1. 将要修改的aar文件复制到libs文件夹下
2. 在`build.gradle`文件内填写该文件的全名
3. 在`excludeAar.gradle`文件内填写要剔除的包名或类名，以及打包输出的文件名
4. 在`rule.txt`文件内写入要替换的包名
5. 执行`./gradlew excludeAar`
6. 生成的新aar在`./build/excludeaar`文件夹下