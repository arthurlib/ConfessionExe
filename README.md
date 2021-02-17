# ConfessionExe

![view](./view.gif)

> 下载

[download Confession.exe](https://github.com/zhuzhenyuan/ConfessionExe/releases/download/first/Confession.exe)

> 打包

* pyinstall + python3.8

1. 先执行 `yinstaller -F -w -i res/red.ico main.py`, 会生成main.spec文件
2. 修改main.spec文件， Analysis中的datas 修改为`datas=[('res', 'res')]`, EXE中添加一行 `console=False , icon='res/red.ico')`
3. 再次打包 `pyinstaller -F -w -i main.spec`
