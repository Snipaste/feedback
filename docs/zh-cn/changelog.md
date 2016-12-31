# 更新日志

## v1.11.0
> 2017.01.01

### 新增：
* 记忆多个历史截图区域 [#249](https://github.com/liulex/Snipaste-Feedback/issues/249)
  * 截图时通过多次按下 <kbd>R</kbd> 或 <kbd>Shift</kbd> + <kbd>R</kbd> 来选择
  * 数量等于截图的最大历史记录数
* 增加一个备用更新源
* 在更新器对话框增加“重新检测”按钮
* [命令行选项](https://github.com/liulex/Snipaste-Feedback/wiki/%E5%91%BD%E4%BB%A4%E8%A1%8C%E9%80%89%E9%A1%B9)：`--snip-whiteboard` 白板模式
* 选项：自定义截图时回车键的功能
* 选项：以鼠标指针为中心缩放贴图 [#277](https://github.com/liulex/Snipaste-Feedback/issues/277)
* 选项：重置贴图操作对缩略图也起作用 [#280](https://github.com/liulex/Snipaste-Feedback/issues/280)
* 选项：贴图上的拖放操作可保留原贴图
* 荷兰语翻译（感谢 **Stephan Paternotte**）

### 修复：
* 对 Nsight 控件进行元素检测导致其崩溃 [#290](https://github.com/liulex/Snipaste-Feedback/issues/290)
* 特定条件下，截图结束后未解除对 <kbd>Win</kbd> 的屏蔽 [#272](https://github.com/liulex/Snipaste-Feedback/issues/272)
* 启动后第一次在截图时按下 <kbd>Tab</kbd> 没有效果
* 检测更新时的一些逻辑错误

### 改进：
* 即使在编辑状态，也可以通过空格键隐藏/显示标注工具条了
* 灰度颜色的 Hue 由 -1 改为 0
* 多处细节优化 :)

## v1.10.5
> 2016.12.10

### 新增：
* 颜色卡片增加 HSV 和 HSI 格式

### 修复：
* 从 Chrome 复制的文字粘贴到文字标注框后显示出错 [#257](https://github.com/liulex/Snipaste-Feedback/issues/257)
* 从 Android Studio 复制的文字转化为贴图后丢失了格式 [#266](https://github.com/liulex/Snipaste-Feedback/issues/266)
* 特定条件下启动，无法对置顶窗口截图 [#269](https://github.com/liulex/Snipaste-Feedback/issues/269)
* 贴图之间的层叠次序在重启后有可能没有正确恢复

### 改进：
* "开机启动"已勾选的情况下，启动时若发现开机启动快捷方式丢失，自动尝试重新生成

## v1.10.4
> 2016.12.05

### 修复：
* 特定条件下添加/移除显示器没有被检测到 [#233](https://github.com/liulex/Snipaste-Feedback/issues/233)
* 对 GIF 文件进行拖拽出错 [#260](https://github.com/liulex/Snipaste-Feedback/issues/260)
* 特定条件下放大镜消失
* 特定条件下无限弹出更新通知

## v1.10.3
> 2016.12.01

### 新增：
* 全新的 [用户手册](https://docs.snipaste.com/zh-cn)
  * 使用 <a href="https://docsify.js.org/#/zh-cn" target="_blank">docsify</a> 生成

### 修复：
* 系统设置“拖动时显示窗口内容”未勾选时，无法移动贴图
* 贴出的文件路径无法复制其文字
* 对线条的锚点进行 <kbd>Shift</kbd> 拖动时无效
* [#253](https://github.com/liulex/Snipaste-Feedback/issues/253)

### 改进：
* 取消对 画笔/马赛克/橡皮擦 的整体移动操作，以防止连续标注时误触

## v1.10.2
> 2016.11.28

### 新增：
* 可随时二次编辑文字标注
* 折线、画笔、马赛克、橡皮擦等形状可以整体拖动
* <kbd>鼠标左键</kbd>按下 + <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> 可逐像素移动贴图 [#211](https://github.com/liulex/Snipaste-Feedback/issues/211)
* [命令行选项](https://docs.snipaste.com/zh-cn/command-line-options)：`--paste-files` 可指定文件夹
* [高级设置](https://docs.snipaste.com/zh-cn/advanced-configs)：snip/exclude_from_detection
* [高级设置](https://docs.snipaste.com/zh-cn/advanced-configs)：snip/crashes

### 修复：
* 程序开机自启后，如手动点检查更新，导致首选项窗口等无响应 [#242](https://github.com/liulex/Snipaste-Feedback/issues/242)
* 以管理员身份启动时无法响应命令行调用 [#240](https://github.com/liulex/Snipaste-Feedback/issues/240)
* 特定条件下进入截图后窗口自动选取失效 [#123](https://github.com/liulex/Snipaste-Feedback/issues/123)


### 改进
* 几处细节修正

## v1.10.1
> 2016.11.22

### 修复：
* 程序一运行即崩溃（小部分用户）
* 回放截图历史时显示有误
* 在线更新后未弹出更新成功的通知

## v1.10.0
> 2016.11.22

### 新增：
* 支持 [命令行选项](https://docs.snipaste.com/zh-cn/command-line-options)
* 截屏时，允许在编辑模式调整选区 [#211](https://github.com/liulex/Snipaste-Feedback/issues/211)
* 全部标注形状支持 <kbd>Shift</kbd> 功能
* “折线“新增直线模式：按住 <kbd>鼠标左键</kbd> 并拖动即可
* 托盘图标右键菜单中新增 "帮助" 菜单
* 在贴图上按 <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>C</kbd> 可直接复制纯文本（如果该贴图是由文本转换而来）
* 点击快速保存的气泡通知，可以在文件资源管理器查看文件 [#220](https://github.com/liulex/Snipaste-Feedback/issues/220)
* 贴图右键菜单，"在文件夹中查看" [#223](https://github.com/liulex/Snipaste-Feedback/issues/223)
* 选项：以管理员身份开机启动
  * 以便可以在管理员权限的窗口响应快捷键
* 选项：设置代理服务器
* 选项：启动后检测更新的延时
* 选项：每隔一段时间检测更新
* 选项：检查更新时包括 beta 版
* 选项：关闭文字转图片

### 改进：
* **大幅提升截屏效率**
* 重绘所有图标，不再使用图标字体
* 截图时直接贴图的快捷键由 <kbd>Ctrl</kbd> + <kbd>W</kbd> 更改为 <kbd>Ctrl</kbd> + <kbd>T</kbd>
* 轻微调整了放大镜的绘制
* 截屏时工具条的位置调整策略
* 截屏时选区大小标签的位置调整策略

### 修复：
* 增强版托盘菜单中，"显示/隐藏所有贴图" 绑定了错误的动作 [#202](https://github.com/liulex/Snipaste-Feedback/issues/202)
* 连续切换贴图组可能导致无法贴出新图 [#199](https://github.com/liulex/Snipaste-Feedback/issues/199)
* 许多小 bug

## v1.9.2
> 2016.10.31

### 修复：
* 移动贴图到另一个组，导致另一个组的贴图丢失 （存在于 1.9.0 及 1.9.1）
* 将贴图移动到由旧版程序建立的一个组之后，切换过去导致程序崩溃
  * **此次更新后，请循环切换到每个贴图组，以升级贴图的历史记录文件**
* 贴图移组之后，贴图计数可能没有正确更新

### 改进：
* 贴图移动到另一个组之后，将位于原组的所有贴图之上

## v1.9.1
> 2016.10.27

### 修复：

* 贴图操作的用户配置在升级后丢失

### 改进：

* 手动保存文件也应用文件命名规则（但后缀将依然沿用上一次手动保存时候的）

## v1.9.0
> 2016.10.26

### 新增：

* 自定义图片文件命名规则 [#98](https://github.com/liulex/Snipaste-Feedback/issues/98)
* 延时截屏 [#181](https://github.com/liulex/Snipaste-Feedback/issues/181)
* 放大镜可见时，按 <kbd>Shift</kbd> 切换颜色格式 [#187](https://github.com/liulex/Snipaste-Feedback/issues/187)
* 拖选选区时按住空格键可移动选区 [#192](https://github.com/liulex/Snipaste-Feedback/issues/192)
* 巴西葡萄牙语翻译（感谢 **Igor Rückert**）
* 波兰语翻译（感谢 **Wirus deleted my username**）

### 修复：

* 连续切换贴图组导致崩溃
* 选项对话框中，改变文字转图片的设置后，其预览图片没有相应更新
* 对标注进行"重做"后，有可能颜色恢复错误
* 多处逻辑错误

### 改进：

* 保证历史记录文件保存时的完整性
* 大大提升连续切换贴图组的效率
* 在自定义贴图操作中禁用 <kbd>Shift</kbd> + <kbd>左键</kbd>（因与贴图对齐冲突）
* 快速保存时在气泡通知中显示文件保存路径
* 记忆选项对话框的位置及当前标签
* 选项对话框尺寸发生变化时使用过渡动画

## v1.8.8
> 2016.10.16

### 修复：

* 快速保存目录路径处理出错（错误地使用了其上一级目录，存在于 1.8.6 及 1.8.7）
* 重启 Snipaste 后没有记住之前的箭头和文字的缩放
* 放大镜出现时，短暂显示了上一次放大镜的内容

## v1.8.7
> 2016.10.15

### 修复：

* 无法播放音效

## v1.8.6
> 2016.10.15

### 新增：

* 选项：截图完成后播放音效
* 编辑时按下 Alt+C 将从屏幕取色并应用到画笔

### 改进：

* 标注被”重做”后自动切换到相应形状的编辑状态，方便二次编辑
* 快速保存路径支持相对路径

## v1.8.5
> 2016.10.13

### 新增：

* 支持包含 <kbd>PrtSc</kbd> 的全局快捷键

### 改进：

* 更改 "Meta" 键的名称为 "Win"

## v1.8.4
> 2016.10.12

### 新增：

* 选项：自定义贴图上的鼠标操作
 * 注意：关闭贴图的默认操作重新调整为"双击"，切换缩略图模式为"Win+左键单击"
 * 如不习惯，请自行设置
* 选项：自定义输出的图片质量
* 更新了内置快捷键列表，并增加了“复制”按钮
* 在贴图上按 <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> 唤出选项窗口
* [高级设置](https://docs.snipaste.com/zh-cn/advanced-configs)：General/high_process_priority
* [高级设置](https://docs.snipaste.com/zh-cn/advanced-configs)：snip/do_not_omit_synthesized_c
* 日语翻译 (感谢 **鳳凰院カミ**)

### 修复：

* 连续切换贴图组导致程序崩溃
* 缩略图模式的贴图无法闪烁边框
* 贴图默认的不透明度小于 100 时，贴图判重有误

### 改进：

* 截屏时不再屏蔽所有合成按键（以便 ahk 等软件模拟的按键可正常使用）
* 即使“自动检测界面元素”没有勾选，截屏时也可以通过按 Tab 来检测界面元素
* 长度/宽度很小的贴图也可以很容易被移动了

## v1.8.3
> 2016.10.02

### 修复：

* v1.8.2 使用了错误的截图历史记录文件夹
* 双击托盘图标导致 Snipaste 被强制退出

### 改进：

* 当前激活的贴图窗口的阴影将使用主题色

## v1.8.2
> 2016.09.30

### 新增：

* [高级设置](https://docs.snipaste.com/zh-cn/advanced-configs)：历史记录文件夹位置

### 修复：

* 在线更新后 Snipaste 没有自动重启（部分用户）
* 从托盘菜单关闭组之后，菜单没有自动隐藏

### 改进：

* 从增强版托盘菜单中移除了“重启”
* 启动时检查并移除历史记录文件夹中未使用到的文件夹

## v1.8.1
> 2016.09.29

### 修复：

* 部分选项在程序重启后没有生效
* （XP）开机启动的快捷键方式在非英文系统没有被成功创建

### 改进：

* 当 config.ini 不可写入时弹出通知提示

## v1.8
> 2016.09.28

### 新增：

* 贴图之缩略图模式（双击它）
* 选项：缩略图大小
* "恢复默认" 按钮
* 可以设置记号笔颜色的透明度了

### 修复：

* 最大化窗口及全屏窗口的范围检测
* 某些高分屏的窗口检测出错
* 双屏（主屏在下，两个屏幕边缘没有对齐）的截屏问题
* 标注形状的控制框被保存到了图像上
* 当颜色为半透明时，矩形/椭圆/折线/画笔 的绘制问题

### 改进：

* 小的颜色按钮不再改变当前颜色的透明度

## v1.7.3
> 2016.09.19

### 修复：
* 识别全屏窗口时没有把任务栏区域包括进去
* （XP）kernel32.dll 错误
* （XP）无法设置全局快捷

### 改进：
* 标注时记住箭头的尺寸
* 启动后恢复上一次的箭头尺寸及文字大小
* 快速保存目录可以手动编辑了
* 窗口检测时忽略不可点击的（透明）窗口
* （XP）消除启动后第一次截图时的窗口动画

## v1.7.2
> 2016.09.17

### 修复：
* 截图时能看到截图窗口的任务栏图标一闪而过
* 一定条件下，刚开始截图时截图区域就被自动确定了
* 截图时光标形状没有及时更新
* 贴图窗口吸附失效（按住 <kbd>Shift</kbd> 键，然后移动贴图窗口并对齐到另一个窗口，然后释放鼠标按键）

## v1.7.1
> 2016.09.15

### 修复：
* "无可用更新"对话框被选项对话框挡住
* 启动时某些 Win 7 x64 用户提示缺少 msvcr120.dll

### 改进：
* 消除截图时直接贴图的延迟

## v1.7
> 2016.09.15

### 新增：

* 自动更新模块
* 截屏时按下 <kbd>Tab</kbd>，可在选取窗口/选取元素之间切换
* 在贴图上按 <kbd>3</kbd> <kbd>4</kbd> 将图像进行镜像翻转
* 选项：截屏时捕捉光标（截图时可按 <kbd>`</kbd> 来切换）
* 选项：截图时单击中键将截图贴到屏幕上 [#63](https://github.com/liulex/Snipaste-Feedback/issues/63)
* 选项：贴图默认透明度 [#96](https://github.com/liulex/Snipaste-Feedback/issues/96)
* 选项：以 Windows Bitmap 格式将图像复制到剪贴板 [#20](https://github.com/liulex/Snipaste-Feedback/issues/20)
  * 如果发现图像无法粘贴到某些应用（如 Skype、UWP 版微信），请打开此选项，但同时会丢失图像的透明通道
* 选项：增强版托盘菜单
* 选项：自定义截屏时的边框宽度
* 选项：在放大镜中显示/隐藏边框
* 选项：在放大镜中显示/隐藏遮罩
* 选项：进入截屏后默认显示全屏十字线
* 选项：截屏时如有其他程序的窗口激活，是否自动退出截屏
* 选项：在贴图右键菜单显示助记键
* 选项：切换到另一分组时自动闪烁贴图

### 修复：

* 截屏时与词典软件的取词、划译等功能的冲突（已测试必应词典、有道词典、QTranslate） [#64](https://github.com/liulex/Snipaste-Feedback/issues/64)
* 自动检测界面元素时可能导致的截图无响应 [#95](https://github.com/liulex/Snipaste-Feedback/issues/95) [#116](https://github.com/liulex/Snipaste-Feedback/issues/116)
* 自动检测窗口对少部分用户无效 [#61](https://github.com/liulex/Snipaste-Feedback/issues/61)
* 某些情况下开始截图后没有获取到键盘焦点 [#114](https://github.com/liulex/Snipaste-Feedback/issues/114)
* 特定操作下截图后贴图导致程序崩溃 [#119](https://github.com/liulex/Snipaste-Feedback/issues/119)
* 试图贴出剪贴板中的超大文件时拷贝副本造成机器卡顿 [#102](https://github.com/liulex/Snipaste-Feedback/issues/102)
* 在触屏上用手指无法正常截图
* <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>S</kbd> 有时候没反应 [#42](https://github.com/liulex/Snipaste-Feedback/issues/42)
* 画矩形/椭圆时按下 <kbd>Shift</kbd>，工具条的图标有时没有同步变化 [#53](https://github.com/liulex/Snipaste-Feedback/issues/53)
* （某种设置下的）高分屏截屏时图片模糊 [#74](https://github.com/liulex/Snipaste-Feedback/issues/74)
* （某种设置下的）高分屏贴图显示错误 [#74](https://github.com/liulex/Snipaste-Feedback/issues/74)
* 半透明文字绘制有误
* 橡皮擦及马赛克在背景半透明时绘制有误
* 某些条件下导致贴图重复
* 直接把截图贴到屏幕时，贴图没有被激活（选项有勾选的情况下）
* 保存截图时，边框被画进了截图

### 改进：

* 拖动文字框时默认不旋转，按下 <kbd>Ctrl</kbd> 才可以旋转
* 记忆上一次手动保存图片时的后缀名
* 固定箭头宽度（不再随箭头长度而增加），但用户可通过 <kbd>鼠标滚轮</kbd> 或 <kbd>1</kbd> <kbd>2</kbd> 改变其大小
* 统一截图和贴图的快速保存目录
* 直接点击托盘右键菜单上的分组名切换到分组，同时，关闭、重命名分组请在分组名上右键
* 在大的颜色按钮上增加一个彩色三角，以表示点击后可自定义颜色（By Fubuki）
* “隐藏”单张贴图现在称为“关闭”贴图，以和“隐藏所有贴图”区分开
* 截图界面可见时点击托盘图标将强制退出 Snipaste （以防止万一截图卡住时无法退出 Snipaste）
* 双击空的文字编辑框，也可以直接保存截屏了
* 放大镜将根据当前屏幕的 DPI 自动调整缩放

## v1.6
> 2016.08.10

### 新增：

* 选项：取 Hex 颜色值时不复制 # 
* 镂空箭头样式

### 修复：

* 自动探测窗口范围功能，对 Windows 标准样式窗口，识别范围大了一圈
* 自动探测窗口范围功能，对 QQ 窗口，识别范围大了一圈
* 从 Chrome 复制的带特定格式的 HTML 文本，贴出来的图片可能出错
* 屏幕 150% DPI 时，颜色按钮的大小不对
* 放大镜在贴图窗口上移动时有明显延迟

### 改进：

* 更新了部分图标（感谢 像素君）

## v1.5
> 2016.08.08

### 新增：

* 截图、贴图可快速保存到指定目录（按下 <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>S</kbd>，或 <kbd>Shift</kbd> + “保存”按钮）
* 在自动选取窗口区域状态，按下空格键可确定区域
* 截屏时在光标处绘制全屏的十字标线（需按住Alt）
* 截屏时按下 <kbd>Ctrl</kbd> + <kbd>A</kbd> 快捷键，可将截屏区域选择为全屏
* “内置快捷键”窗口（在 选项窗口-热键 标签下）
* 发送截图/贴图到打印机（没有按钮，只有通过 <kbd>Ctrl</kbd> + <kbd>P</kbd>）
* 选项：在放大镜中显示操作提示（默认开启）
* 选项：取色器使用 Hex 颜色值
* 德语翻译（感谢 Samuel Marcius）
* 希腊语翻译（感谢 geogeo.gr）
* 瑞典语翻译（感谢 Åke Engelbrektson）

### 修复：

* 部分快捷键设置显示设置成功，但实际上并没有效果（除 <kbd>PrtScr</kbd> 以及被系统/其他应用程序占用的快捷键，其他快捷键应可顺利被设置）
* 默认全局快捷键被取消之后在一定条件下可能仍会占用
* 双屏、主屏在右时橡皮擦/马赛克/高斯模糊绘制不正确
* 在自动检测界面元素时可能发生程序崩溃
* 颜色对话框没有被翻译
* 按住Alt在多个贴图窗口之间游走时，有些窗口的放大镜没有被自动隐藏
* “使用截图时的位置”这个选项没有影响到截图时的“贴到屏幕”按钮（或 <kbd>Ctrl</kbd> + <kbd>W</kbd>）

### 改进：

* 从贴图复制颜色值时，闪烁一下放大镜以提示颜色复制成功
* 选项“截图时屏蔽 Win 键”，将只屏蔽 <kbd>Win</kbd> 键单击，不会妨碍 <kbd>Win</kbd> + <kbd>空格</kbd> 等组合键的响应
* 从贴图复制颜色值时，保存图像文件时，下拉菜单可以选多种图片格式
* 给当前正在被设置的快捷键编辑框添加（主题色的）边框
* 在快捷键设置对话框，添加了如何删除快捷键的明显提示
* 更改了默认的全局快捷键设置（如贴图为 <kbd>F3</kbd> 而不是 <kbd>F2</kbd>）（只会影响新用户，老用户不会丢失自己的配置）
* 使用 <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd> 移动贴图（而不是 <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd>），以保持和截屏行为的一致
* 使用系统画图程序（mspaint）的调色板

## v1.4
> 2016.08.01

### 新增：

* XP 版
* 使用退格键删除快捷键
* <kbd>Esc</kbd> 隐藏贴图，<kbd>Shift</kbd> + <kbd>Esc</kbd> 销毁贴图
* 选项：按下贴图键时如有任何贴图在闪烁，自动隐藏所有贴图

### 修复：

* <kbd>Shift</kbd> + <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd> 缩小截取范围时出现负数

## v1.3
> 2016.07.29

### 新增：

* <kbd>Shift</kbd> + <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd> 缩小截图区域
* 繁体中文翻译（感谢 zhtw)

### 修复：

* 多屏（主屏在右）截图时按 <kbd>Alt</kbd> 虚线绘制有误
* 多屏情况下，探测的全屏程序窗口超过当前屏幕范围
* 按住 <kbd>Alt</kbd> 时，双击贴图窗口，贴图窗口隐藏后取色窗口还在并无法关闭

## v1.2
> 2016.07.29

### 修复：

* 多屏（主屏在右）的截图问题
* 切换语言后，托盘图标的 tooltip 的语言没有更新

## v1.0
> 2016.07.28

* 首次发布
