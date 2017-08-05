```
查看元素2种办法：
uiautomatorviewer monitor(其实也是调用的是uiautomatorviewer)


错误：
uiautomatorviewer Unable to connect to adb.Check if adb is installed correctly

解决:
修改uiautomatorviewer.bat
call "%java_exe%" "-Djava.ext.dirs=%javaextdirs%" "-Dcom.android.uiautomator.bindir=%prog_dir%" -jar %jarpath% %* ==>

call "%java_exe%" "-Djava.ext.dirs=%javaextdirs%" "-Dcom.android.uiautomator.bindir=D:\Android\sdk\platform-tools" -jar %jarpath% %*


monitor
错误:
nexpected error while parsing input:Invalid ui automator hierarchy file

解决:
删除monitor-workspace下的内容



pip install -U setuptools
pip install robotframework-appiumlibrary

npm install -g appium-doctor

```
