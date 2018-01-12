# wepy-tony-native
https://mp.weixin.qq.com/debug/wxadoc/dev/quickstart/basic/getting-started.html

### 项目构建
- 小程序官方程序的默认模板


### 代码高亮
- 文件后缀为.WXML，可共用HTML的高亮规则
- 文件后缀为.WXSS，可共用CSS的高亮规则

- 下面提供一些常见IDE或编辑器中实现代码高亮的相关设置步骤以供参考(也可通过更改文件后缀名的方式来实现高亮，详见后文相关介绍)。
- Sublime
    - 1. 打开Sublime->Preferences->Browse Packages..进入用户包文件夹。

    - 2. 在此文件夹下打开cmd，运行git clone git@github.com:vuejs/vue-syntax-highlight.git，无GIT用户可以直接下载zip包解压至当前文件夹。

    - 3. 关闭.wpy文件重新打开即可高亮。

- WebStorm/PhpStorm
    - 1. 打开Settings，搜索Plugins，搜索Vue.js插件并安装。

    - 2. 打开Settings，搜索File Types，找到Vue.js Template，在Registered Patterns添加*.wpy，即可高亮。

- Atom
    - 1. 在Atom里先安装Vue的语法高亮 - language-vue，如果装过了就忽略这一步。

    - 2. 打开Atom -> Config菜单。在core键下添加：


```Atom
customFileTypes:
   "text.html.vue": [
      "wpy"
   ]
```

- VS Code
    - 1. 在 Code 里先安装 Vue 的语法高亮插件 Vetur。

    - 2. 打开任意 .wpy 文件。

    - 3. 点击右下角的选择语言模式，默认为纯文本。

    - 4. 在弹出的窗口中选择 .wpy 的配置文件关联...。

    - 5. 在选择要与 .wpy 关联的语言模式 中选择 Vue。

- VIM
    - 1. 安装 Vue 的 VIM 高亮插件，例如 posva/vim-vue。

    - 2. 配置 .wpy 后缀名的文件使用 Vue 语法高亮。

```vim
au BufRead,BufNewFile *.wpy setlocal filetype=vue.html.javascript.css
```

### app.json
文件名不需要写文件后缀，因为框架会自动去寻找路径下 .json, .js, .wxml, .wxss 四个文件进行整合。

```文件名不需要写文件后缀，因为框架会自动去寻找路径下 .json, .js, .wxml, .wxss 四个文件进行整合。
https://mp.weixin.qq.com/debug/wxadoc/dev/framework/config.html
```



