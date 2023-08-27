# ILRuntimeU3D
Unity3D demo project for ILRuntime

这个是ILRuntime的U3D示例工程


# 调试插件
ILRuntime提供了一个支持Visual Studio 2015、Visual Studio 2017、Visual Studio 2019、Visual Studio 2022和VSCode的调试插件，用来源码级调试你的热更脚本。
你可以在Visual Studio和VS Code的插件商店中搜索ILRuntime安装调试插件。

# Visual Studio调试插件使用方法如下：

安装ILRuntime调试插件，并重新启动Visual Studio
确保dll和pdb都加载完毕。
运行Unity工程，并保证执行过appdomain.DebugService.StartDebugService();来启动调试服务器
用VisualStudio打开热更DLL项目
点击菜单中的Debug->Attach to ILRuntime按钮。注意,不是“附加Unity调试程序”
在弹出来的窗口中会列出可以调试的实例，如果没有显示想要调试的实例可以点击刷新按钮进行刷新
点击OK按钮后，即可像UnityVS一样下断点调试

# VS Code调试插件使用方法如下：
从VS Code插件商店安装调试插件
确保dll和pdb都加载完毕。
运行Unity工程，并保证执行过appdomain.DebugService.StartDebugService();来启动调试服务器
用VS Code打开热更DLL项目
F5新建调试Profile
在弹出来的窗口中会列出可以调试的实例，如果没有显示想要调试的实例可以点击刷新按钮进行刷新
选择需要调试的实例按确定，即可像UnityVS一样下断点调试


# 注意点
打开工程如果有错误，先把错误代码注释掉，然后重新生成解决方案；在Hot工程里面引入加入Unity工程的XIL-master\Library\ScriptAssemblies\Assembly-CSharp.dll，最后再把刚才注释的代码解注就可以了。
