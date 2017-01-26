# 高级设置

这些是没有提供用户界面的高级设置，请小心设置。

## 设置方法

1. 关闭 Snipaste
1. 使用文本编辑器打开程序目录下的 config.ini
1. 在相应的组（中括号包围的即**组名**）下添加你所需的选项
 * 分号后面的为注释，无需添加
1. 保存并关闭 config.ini
1. 启动 Snipaste

## [General]

    ; 设置历史记录文件夹 (>= v1.8.2)
    ; Snipaste 不会为你自动创建文件夹，请自行确保文件夹存在，不存在将自动使用 ./history
    ; 斜杠请使用 / 或者 \\
    ; 如路径中存在空格，无需使用引号; 不支持中文路径
    ; 相对路径示例：
    ; abc
    ; ./abc
    ; ../abc
    ; 绝对路径示例：
    ; D:/configs/sphistory
    ; D:\\abc def\\history

**history_dir=c:/abc**

    ; 隐藏托盘图标 (>= v1.8)
    ; 有效值：true, false

**hide_tray_icon=true**

    ; 以高优先级启动进程 (>= v1.8.4)
    ; 此选项为 Windows 独占
    ; 有效值：true, false

**high_process_priority=true**

## [Snip]

    ; 不屏蔽模拟的 C 键 (>= v1.8.4)
    ; 大部分取词软件的划译功能是通过鼠标松开时自动发送 Ctrl + C 来实现的，为防冲突，Snipaste 需要屏蔽模拟的 C 键
    ; 如果此功能反而妨碍了你的正常使用（如 GoldenDict 用户），可以设置为 true
    ; 此选项为 Windows 独占
    ; 有效值：true, false

**do_not_omit_synthesized_c=true**

    ; 将某些程序的窗口从窗口检测中排除 (>= 1.10.2)
    ; 如使用 LICEcap 进行屏幕录制的时候，LICEcap 自身的窗口会被检测到，从而无法检测到 LICEcap 底下窗口的元素
    ; 这时可将 licecap.exe （大小写无关）加进这里
    ; 多个程序名称请以逗号分割
    ; 此选项为 Windows 独占

**exclude_from_detection=a.exe, b.exe**

    ; 对某些程序的窗口使用另一种界面元素检测算法 (>= 1.10.2)
    ; 对某些程序的窗口进行界面元素检测时，可能会导致 Snipaste 无响应或崩溃
    ; 这时可将它们的程序名称加进这里，Snipaste 会以另一种方法尝试进行元素检测
    ; 这种方法不太可能造成程序崩溃，但同时能检测到的元素略少一些
    ; 多个程序名称请以逗号分割
    ; 此选项为 Windows 独占

**crashes=a.exe, b.exe**