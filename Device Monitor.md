# mac Android Device monitor no response
1. 因为jdk版本不对---使用1.8.0_151 及以下的版本解决
2. Android/sdk/tools/lib/monitor-x86_64/plugins/org.eclipse.swt.cocoa.macosx.x86_64_3.100.1.v4236b.jar版本太低，更新jar。下载
http://ftp.yz.yamagata-u.ac.jp/pub/eclipse/eclipse/downloads/drops4/R-4.7.3a-201803300640/swt-4.7.3a-cocoa-macosx-x86_64.zip
https://download.eclipse.org/eclipse/downloads/index.html
解压后，吧swt.jar复制到Android/sdk/tools/lib/monitor-x86_64/plugins/目录下替换原来的org.eclipse.swt.cocoa.macosx.x86_64_3.100.1.v4236b.jar

# mac 不能启动Android Device monitor
因为Android Device monitor需要监听8700端口，这个端口被Android studio占用。
需要kill android studio进程
