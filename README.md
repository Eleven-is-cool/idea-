#破解idea  
① : 将`https://account.jetbrains.com:443 www.jetbrains.com`，加入hosts（[查看如何修改host](https://blog.csdn.net/iteen/article/details/83274623)）   

② : 打开cmd终端，输入`ipconfig /flushdns`，然后回车刷新dns缓存  
③ : 在桌面右击idea图标打开文件位置，将jar文件拷贝到bin目录  
④ : 用IDE修改修改bin目录下的`idea.exe.vmoptions``idea64.exe.vmoptions`，增加代码`-javaagent:（jetbrains-agent.jar的绝对路径）`  
⑤ : 打开IDE，选择 License Server 然后点击
Discover Server，输入`http://jetbrains-license-server`，点击Activate就可以了。
