# Lazarus  和 FreePascal 的相关资料

## Lazarus 使用优化

###  一体式窗口：
* 菜单Package->Install/Uninstall Packages ...

* 右侧选择安装AnchorDockingDsgn和dockedformeditor这2个控件，点Install selection或双击

* 点Save and rebuild IDE重新构建，IDE重启之后就是一体式的窗口了(构建配置文件选择优化的IDE)

* 拖动子窗口顶部空白块状，会自动吸附，调整为自己喜欢的布局，重启IDE即可

### 项目文件查看： 
* 菜单->项目->项目查看器，弹出项目查看器窗口，拖动该窗口头部空白块，放置到主窗口右侧。
* 调整完成后可以打开菜单Tools->Desktops 保存当前活动桌面布局

### 关闭自动保存布局功能：菜单Tools->Desktops ...，去掉Auto save active desktop的勾选

### 语法高亮：
* 菜单工具->选项->编辑器->显示->颜色->选择Delphi

### 代码提示：
* 菜单工具->选项->编辑器->键盘映射->Code Tools命令->标识符自动完成  选择Ctrl + N  

### 开启代码结构匹配连线功能：

* 菜单工具->选项->编辑器->显示->标记和匹配->结构体轮廓线（全局）

### 去掉右线：菜单工具->选项->显示->边界边栏->去掉“显示右线”勾选

### 自动删除空方法：
* 菜单工具->选项->编辑器->补全和提示->自动移除空方法
* 当保存时会自动删除空的过程/函数
 
### 提高自动代码完成的提示速度：
* Tools->Options-->Editor-->Completion and Hints-->Delay for completion box-->调到最左边
 
### 直接跳到方法体而不是声明：
* 在IDE中按Ctrl+鼠标左键跟踪函数或属性时，默认跳到了申明部分，按下面的方法设置后就能跳到对应的实现部分的代码
* 菜单工具->选项->Codetools->常规->直接跳到方法体

### 恢复lazarusd局：
* lazarus使用anchorDocking和dockedformeditor后，很容易因使用时不小心拖动form后ide布局越调越的情况，经模索发现将config_lazarus文件夹environmentoptions.xml的AnchorDocking节点删除后，再运行lazarus就可以恢复为默认的布局。

### 快捷键
* 格式化代码：选中多行Ctrl+D

* 代码补全:Ctrl+W

* 模板编辑: Ctrl+J，然后输入class，回车。

* 多行缩进:
向左 -> Ctrl+U               
向右 -> Ctrl+I（可选中多行代码）

* 多行注释：Ctrl+/

* 查找被引用：Ctrl + Shift + i

### 批量修改单词:
* 先选中要修改的一段代码，等左边的笔图标出现后，点击编辑器左边显示行号左边的那支笔。这个时候你可以输入test1，变量test就全部改为test1，还可以按下tab跳到下一个单词。