# 故障排除

以下为运行 Snipaste 可能遇到的错误及其解决方案。

## Windows

### 运行后遇到提示计算机中丢失 api-ms-win-crt-runtime-l1-1-0.dll 错误
* 请根据操作系统的版本（32位/64位），下载并安装适合您系统版本的 [微软 Visual C++ 2015 可再发行组件包](https://www.microsoft.com/zh-CN/download/details.aspx?id=48145)
* 如果没有权限安装 VC2015 或安装失败，也可以下载相应压缩包（[32位](https://dl.snipaste.com/vc2015-dll-x86-cn) | [64位](https://dl.snipaste.com/vc2015-dll-x64-cn)），解压后将所有 dll 放到 Snipaste 目录下

### Windows XP 32位运行后提示 Snipaste.exe 不是有效的 Win32 应用程序
* 请 [下载](https://zh.snipaste.com/download.html) 针对 XP 系统的 Snipaste 程序

### Windows SmartScreen 筛选器已阻止启动一个未识别的应用
* 请点击“更多信息”，然后点击“仍要运行”
* 这只是因为 Snipaste 尚未进行数字签名，只要是从[官网](https://zh.snipaste.com)下载的，请放心使用

### 检查更新时提示 `网络错误: 99`
* 通常是由于程序目录下缺少 libeay32.dll 和 ssleay32.dll，请下载完整包并完整解压覆盖

### 运行后提示缺少 Qt5\*\*\*.dll 错误
* 请确保网站提供的压缩包中的每个文件都在本地的程序目录中
* Snipaste 版本升级时可能会增加新的 dll，所以不建议通过手动替换 .exe 的方式升级，请尽可能使用在线更新

### 无法截取菜单，一按截图快捷键菜单就消失了
* 在 Windows 系统，<kbd>Alt</kbd> 按下时菜单会自动消失。因此，如果需要截取菜单，截图快捷键不要包含 <kbd>Alt</kbd> 即可
* 也可以使用延时截屏

### 重启 Snipaste 之后，配置文件又回到了默认状态
* 原因：Snipaste 无法写入程序目录下的 config.ini
* 因此解决 config.ini 的写入权限即可：
 * 不要把 Snipaste 放到 C:\Program Files\ 或者 C:\Program Files(x86)\ 目录下，这种目录下的文件通常需要管理员权限才能写入
 * 如果并没有把 Snipaste 放到如上的目录，但问题依旧，可能是磁盘权限的问题（如系统升级就可能导致）。因原因不尽相同，请自行使用搜索引擎解决磁盘权限问题
 * 如问题仍然无法解决，请使用管理员权限运行 Snipaste

### 无法设置快捷键为某些快捷键（如某些带 <kbd>Win</kbd> 的组合键）
* 部分带 <kbd>Win</kbd> 的组合键被系统占用了
* 同理，已经被其他程序占用的的快捷键，也是不能为 Snipaste 所用的，请先在其他软件解除掉
  * OneDrive 可能占用 <kbd>PrintScreen</kbd>，需取消勾选：`屏幕快照 - 自动将我捕获的屏幕截图保存到 OneDrive`

### 有时候快捷键不响应
* 这是 Windows 的权限问题。如果 Snipaste 没有以管理员权限运行，而当前窗口是以管理员身份运行的，那么快捷键会失效
* 解决办法：
  * 点击一下任务栏或者其他非管理员运行的窗口，再按快捷键
  * 或者，以管理员身份运行 Snipaste

### 开机启动失效
* 如手动在 Snipaste.exe 右键属性里勾选了“以管理员身份运行此程序”，那么普通方式的开机启动是不会生效的
  * 如有此类需要，请使用 Snipaste 自带的以管理员身份开机启动（版本 v1.10.0 以上）

### 截图时无法自动选取 Chrome 浏览器窗口的页面元素
* 在 Chrome 浏览器地址栏中输入并打开 `chrome://accessibility`，勾选 `Global accessibility mode`
  * 每次重启 Chrome 都需要重新打开这个选项
  * 如果希望每次打开 Chrome 时自动启用 `Global accessibility mode`，请给 Chrome 的启动命令加上 `--force-renderer-accessibility`
  * 在高分屏下，识别到的元素范围可能有误，此问题暂无法解决
* Firefox 及 IE 浏览器则无需额外设置

### 代码编辑器里带语法高亮的代码，复制后贴出来并没有语法高亮
* 这是因为你复制出来的代码并没有带 HTML 格式
* 若希望贴图中的代码被语法高亮，请使用带 HTML 格式复制的代码编辑器
 * 个人推荐使用 Visual Studio，并安装 Productivity Power Tools 插件，打开插件的 "HTML Copy" 功能，这样贴出来的图片可以和编辑器渲染的一样

### 贴图无法拖动超过屏幕上边界
* 系统属性 - 高级 - 性能设置 - 视觉效果 - 勾选"拖动时显示窗口内容" - 确定

![](https://cloud.githubusercontent.com/assets/2010459/18747273/018a85c2-80ff-11e6-9e84-9c42348ffd77.png)
