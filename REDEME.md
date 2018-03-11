# About mainfest.json
name 和 version 是必须的；
Chrome 应用的开发者当前必须指定 'manifest_version': 2；
permissions 声明需要申请的权限，比如访问浏览器选项卡（tabs）、浏览器通知（notifications）等，可以根据需要添加，目前，我们的实例主要是从 GitHub 获取数据并展示数据，暂时不需要申请什么 permissions；
browser_action 指定扩展的图标放在 Chrome 工具栏中，它定义了扩展图标文件位置（default_icon）、悬浮提示（default_title）和点击扩展图标所显示的页面位置（default_popup）；
background 是一个长时间运行的脚本，在扩展的整个生命周期都存在，用于管理一些任务和状态；
options_page 属性定义了扩展的设置页面，配置后在扩展图标点击右键可以看到选项 ，点击即打开指定页面;
content_scripts 则是直接注入页面的脚本。
