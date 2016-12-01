# 命令行选项

Snipaste 1.10 开始，支持带命令行选项调用 Snipaste 的部分功能。

由于 Snipaste 首先是贴图软件，目前所有命令行选项都需要 Snipaste 先在后台运行。

即，如果当前没有运行 Snipaste，所有命令行选项会被忽略，转为正常启动 Snipaste.

Snipaste 启动之后，再带命令行参数启动 Snipaste，才会执行响应的功能。


# 调用方法
    snipaste.exe [OPTION]

> 示例：

> 通过将快捷方式目标设定为 `/path/to/your/Snipaste.exe --snip-full`，或者通过其他程序调用，即可开始全屏截图。

> 注意：暂不支持同时调用截图选项与贴图选项

# 截图选项

    --snip                            开始截屏
    --snip X Y WIDTH HEIGHT           开始截屏，并把选区左上角设为 (X, Y)，
                                      宽度为 WIDTH，高度为 HEIGHT
    --snip WIDTH HEIGHT               开始截屏，并把选区宽度设为 WIDTH，
                                      高度为 HEIGHT，选区中心为当前的光标位置
    --snip-full                       开始截屏，并把选区设定为全屏
    --snip-last                       开始截屏，并把选区设定为上一次成功截屏的区域
    --snip-delay                      开始延时截屏
    --snip-delay TIME                 TIME 秒后开始截屏

# 贴图选项

    --paste                           将剪贴板内容转化为贴图贴出
    --paste-text TEXT                 将纯文本 TEXT 贴出
                                      (如带有空格需用双引号括起)
    --paste-html TEXT                 将 TEXT 视作 HTML 格式贴出
                                      (如带有空格需用双引号括起)
    --paste-files FILE1 FILE2 ...     将图像文件 FILE1, FILE2 等贴出
    --paste-files FOLDER1 FILE1       将图像文件 FILE1, FILE2, FILE3 等贴出 
      FILE2 FOLDER2 FILE3 ...         如果 FILE1 是个相对路径，那么它是相对于文件夹 FOLDER1 的，
                                      同理 FILE3 是相对于文件夹 FOLDER3.
                                      文件夹路径需要以 / 或 \ 结尾。
    --images-toggle                   显示/隐藏所有贴图
    --images-show                     显示所有贴图
    --images-hide                     隐藏所有贴图
    --switch-next                     切换到下一个贴图组
    --switch GROUPNAME                切换到名称为 GROUPNAME 的贴图组
                                      (如带有空格需用双引号括起)
    --click-through-toggle            打开/关闭贴图的鼠标穿透模式
    --click-through-enable            打开贴图的鼠标穿透模式
    --click-through-disable           关闭贴图的鼠标穿透模式


