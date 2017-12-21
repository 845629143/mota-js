# H5 魔塔样板

## 简介

HTML5 canvas制作的魔塔样板，支持全平台游戏！
**即使完全不会编程的用户，按照模板和说明文档也能很快做出一个魔塔游戏！**

* [Demo / 样板效果](https://ckcz123.com/games/template/)
* [Docs / 使用文档说明](https://ckcz123.github.io/mota-js)

![样板](./docs/img/sample0.png)

## 目录结构

``` bash
├── /docs/           # 文档目录
├── /images/         # 所有图片素材目录
│ ├─ /常用素材/       # 可以被直接替换的素材
│ └─ *.png           # 对应的某个具体的图片素材
├── /libs/           # JS源代码目录
│ ├─ /floors/        # 剧本文件，记录了每个地图的数据和事件
│ ├─ core.js         # 系统核心文件，处理了所有逻辑等事件
│ ├─ data.js         # 记录了勇士的初始化信息、各个全局变量和全局Flag值
│ ├─ enemys.js       # 记录了怪物的信息，包括怪物的数据和特殊属性、伤害计算公式、临界值计算等。
│ ├─ events.js       # 处理事件的文件，所有系统或自定义事件都会在此文件中进行处理
│ ├─ icons.js        # 记录了图标信息，将元件的ID和images目录下的素材图标对应起来
│ ├─ items.js        # 记录了道具的信息，包括道具说明、道具效果等。
│ ├─ maps.js         # 记录了地图信息，负责将数字与元件的ID一一对应起来。
│ └─ ui.js           # UI绘制信息，主要负责绘制各个UI窗口。
├── /sounds/         # 音效目录
├── /常用工具/        # 一些常用工具，可以辅助造塔  
│ ├─ JS代码压缩工具.exe    # 能对Javascript代码进行压缩和整合，从而减少IO请求量。 http://github.com/ckcz123/JSCompressor/
│ ├─ 便捷PS工具.exe        # 能只用复制和粘贴来快速对素材进行PS操作。  http://github.com/ckcz123/ps/
│ ├─ 地图生成器.exe        # 能从一张截图识别出来具体的数字数组，方便复刻已有的塔。 http://github.com/ckcz123/map_generator/
│ └─ 伤害和临界值计算器.exe       # 一个能帮助计算怪物的伤害和临界值的小工具。 http://github.com/ckcz123/magic-tower-calculator/
├── drawMapGUI.html  # 可视化地图编辑工具，能简单地在界面上绘制地图
├── index.html       # 主程序，游戏的入口
├── main.js          # JS程序的入口，将动态对所需JS进行加载
├── style.css        # 游戏所需要用到的样式表
└── 启动服务.exe      # 一个本地的HTTP服务器，也能支撑前端的一些POST请求从而能拓展JS的IO功能。 http://github.com/ckcz123/mota-js-server/
```

## 更新说明

### 2017.12.20
* [x] 新增：本地HTTP服务器。
* [x] 新增：可视化地图编辑工具。
* [x] 新增：便捷PS工具。
* [x] 新增：对Autotile图块的支持。
* [x] 新增：怪物支持多种属性；添加仇恨属性。
* [x] 移除了不再支持的checkBlock，现在对于领域和夹击无需再手动指定可能的点了。
* [x] 新增：单向箭头、感叹号（单次通行）的支持。
* [x] 新增：更多的默认素材，现在对于大多数地图风格无需P图，直接替换即可。
* [x] 部分细节优化，一些已知的Bug进行了修复。

### 2017.12.16

* [x] 新增：战斗过程显示，可以在设置中关闭
* [x] 新增：勇士支持48*32（大图）的行走图
* [x] 新增：更改画面色调
* [x] 新增：文字显示支持自动换行
* [x] 部分修改状态栏UI
* [x] 增添Web的Markdown文档，移除原本的doc和pdf文档。
* [x] 修复若干Bug。

### 2017.12.9

* 发布初版HTML5魔塔样板

## 联系我们

本塔由 [`ckcz123`](https://github.com/ckcz123) （百度ID `艾之葵`）编写。

HTML5魔塔交流群群号： `539113091`

如有其它意见或建议，也可以通过发[issues](https://github.com/ckcz123/mota-js/issues)、或邮件至[ckcz123.com](mailto:ckcz123.com)联系我。
