---
title: 我的 VSCode 插件配置
date: 2019-08-18 09:34:44
tags:
- 软件
- 插件
- 工具
categories:
- 软件
---

## 导读

工欲善其事必先利其器!

工匠想要使他的**工作**做好，一定要先让**工具**锋利。

软件开发者每天接触的就是编辑器，只有把编辑器熟练的掌握才能更好的提升开发效率。

## 拓展插件(Extensions)

1. [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - 插件化的 javascript 代码检测工具，有多种主流的编码风格规则集可供选择,典型的有 [Airbnb](https://link.juejin.im/?target=https%3A%2F%2Fwww.npmjs.com%2Fpackage%2Feslint-config-airbnb)、[Standard](https://github.com/standard/eslint-config-standard) 等代码规范
2. [TSLint](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-typescript-tslint-plugin) - Typescript 的语法高亮，语法提示。
3. [stylelint](https://marketplace.visualstudio.com/items?itemName=shinnn.stylelint) - css 代码检查工具。（标准化 stylelint 的插件，规范 style 代码）
4. [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) - Markdown 编写文档规范检查工具，没有规范是不行的。
5. [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) - 这款插件能实时的识别单词拼写是否有误，并给出提示，不少 bug 都是因为拼写错误导致的。
6. [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer) - 增加代码中括号之间嵌套关系的颜色区分。
7. [Trailing Spaces](https://marketplace.visualstudio.com/items?itemName=shardulm94.trailing-spaces) - 检查代码中多出空格，强迫症必备。
8. [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) - 开发 Vue 必装的一个插件。
9. [JavaScript (ES6) code snippets in StandardJS style](https://marketplace.visualstudio.com/items?itemName=jmsv.JavaScriptSnippetsStandard) - ES6 常用代码片段，Standard 版本。
10. [koroFileHeader](https://marketplace.visualstudio.com/items?itemName=OBKoro1.korofileheader) - 在 vscode 中用于生成文件头部注释和函数注释的插件。
11. [GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) - 一款强大 GIt 源代码管理插件。
12. [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) - 快速启动一个本地服务预览项目。
13. [open in browser](https://marketplace.visualstudio.com/items?itemName=techer.open-in-browser) - 在浏览器中快速打开 html 文件。
14. [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) - VScode 中路径智能补全。
15. [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)  -自动引入 node_modules 中的 JS 路径。
16. [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager) - 项目管理插件。
17. [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync) - 绑定 GitHub 账户进行插件配置备份恢复。
18. [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons) - 为侧边栏文件类型提供相应的图标。

## 个人配置(Settings)

```json
{
  "workbench.editor.showTabs": true, // 控制打开的编辑器是否应显示在选项卡中
  "workbench.iconTheme": "vscode-icons", // 指定工作台中使用的图标主题
  "editor.fontFamily": "Fira code", // 设置字体
  "editor.fontLigatures": true, // 启用/禁用字体连字
  "editor.fontSize": 14, // 字体大小
  "editor.tabSize": 2, // 一个制符表等于的空格数
  "editor.rulers": [80], // 代码长度
  "files.insertFinalNewline": true, // 保存代码自动最后一行添加换行
  "explorer.confirmDelete": false, // 删除文件时要求确认
  "explorer.confirmDragAndDrop": false, // 是否应通过拖放操作要求确认移动文件和文件夹
  "workbench.startupEditor": "newUntitledFile", // 控制在启动时显示哪个编辑器，如果没有从前一个会话恢复。
  "terminal.integrated.fontFamily": "Source Code Pro for Powerline", // 终端设置字体
  "terminal.integrated.fontSize": 14, // 终端字体大小
  "terminal.integrated.shell.osx": "/bin/zsh", // shell 路径
  "terminal.integrated.cursorStyle": "line", // 终端光标的样式
  "git.enableSmartCommit": true, // 没有分阶段更改时提交所有更改
  "git.confirmSync": false, // 在同步git存储库之前确认
  "javascript.updateImportsOnFileMove.enabled": "never", // 在VSCode中重命名或移动文件时，启用/禁用导入路径的自动更新。需要在工作区中使用TypeScript 2.9或更高版本。
  "eslint.autoFixOnSave": true, // 保存的时候根据代码规范自动格式化
  "eslint.validate": [
    "javascript","javascriptreact","typescript","typescriptreact",
    { "language": "vue", "autoFix": true }
  ],
  "eslint.options": {
    "plugins": []
  },
  "vetur.validation.template": false, // 是否使用vetur验证
  "sync.gist": "xxx",
  "sync.autoDownload": false, // 自动恢复编辑器配置
  "sync.forceUpload": true,
  "fileheader.configObj": {
    "autoAdd": false, // 关闭保存自动添加文件注释
    "colon": " ", // 所有注释的冒号改为一个空格，默认为": "
  },
  "fileheader.cursorMode": { //  函数注释
    "description": "",
    "author": "zouzonghua",
    "param": "",
    "return": "",
    "Date": "",
  },
  "fileheader.customMade": { // 头部注释
    "Description": "",
    "Author": "zouzonghua",
    "Date": "Do not edit", // 文件创建时间(不变)
    "LastEditors": "zouzonghua", // 文件最后编辑者
    "LastEditTime": "Do not edit" // 文件最后编辑时间
  },
  "javascript.implicitProjectConfig.experimentalDecorators": true, // 关闭实验装饰器警告
  "window.zoomLevel": 0 , // 窗口缩放级别
  "editor.quickSuggestions": { // 开启注释、字符串 代码提示
    "other": true,
    "comments": true,
    "strings": true
  }
}

```
