## 使用注册表工具实现右键命令清理剪切板

[回到首页](./index.md)

有时候我们不希望保留剪切板的内容，当然使用Ditto之类的剪切板管理工具是一个选择，但如果只是想方便地清理剪切板，基于最小原则，使用右键菜单足以。

使用注册表工具可以编辑右键菜单，路径在`计算机\HKEY_CLASSES_ROOT\Directory\Background\shell\`，新建一个`清理剪切板`的项目，在项目下新建`command`子项目，修改键值为`cmd.exe /c echo off | clip`，保存退出。
