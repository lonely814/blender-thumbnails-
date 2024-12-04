# Blender - 缩略图补丁

在使用 Blender 软件时，可能会遇到这样的困扰：无论是在软件内部进行注册操作，还是通过命令提示符（CMD）使用“blender -r”指令后，都没有任何效果，始终无法显示缩略图。而我们的这个 Blender 缩略图补丁，就能有效解决这一问题。

## 原理代码介绍
以下是相关的原理代码，供有一定基础且希望深入了解其运行机制的用户参考：
```
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID\{D45F043D-F17F-4e8a-8435-70971D9FA46D}]
@="Blender Thumbnail Handler"

[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID\{D45F043D-F17F-4e8a-8435-70971D9FA46D}\InProcServer32]
@="C:\\Program Files\\Blender Foundation\\Blender\\BlendThumb.dll"
"ThreadingModel"="Apartment"
```

## 便捷使用方式
如果您觉得操作代码比较麻烦，也没关系，我们还提供了另一种便捷的解决方案。您可以直接下载我已经编译完成的 EXE 格式文件，只需双击该文件，就能轻松解决 Blender 缩略图无法显示的问题啦。 
