# LoaderShellcode分离免杀(Linux)

模块通过编码shellcode与loadershellcode结合的方式实现免杀.通过将shellcode和loader分开为两个文件来绕过沙箱.

## 操作方法

+ 新建监听(linux)
+ 打开模块,选择对应的监听
+ 运行模块后即会在`文件管理`中生成一个zip文件,包含免杀的elf载荷及对应的C++代码

![](img\Execution_UserExecution_LinuxSplitShellcodeLoader\1.webp)

![](img\Execution_UserExecution_LinuxSplitShellcodeLoader\2.webp)

## 注意事项

模块当前只适配以下载荷:

linux/x86/meterpreter/reverse_tcp

linux/x86/meterpreter/bind_tcp

linux/x64/meterpreter/reverse_tcp

linux/x64/meterpreter/bind_tcp


