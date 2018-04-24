# minapp-slider-left
微信小程序左划删除组件，可能是性能最好、实现最简单的方案，使用官方组件movable-area、cover-view实现

## 预览
+ 已经使用在线上项目，全程基本稳定在60fps,线上项目预览效果：
![image](./doc-img/preview.gif)

+ 你也可以复制下面的小程序代码片段地址,打开微信开发工具,导入代码片段，即可查看效果
```
wechatide://minicode/lUrGBUmn65YS
```

## 使用方式

### 原生小程序中使用，本组件就是用官方提供的组件API开发的，没有任何依赖，参照代码片段中的使用方式使用即可
### [mpvue](https://github.com/Meituan-Dianping/mpvue)中使用
- 首先在mpvue项目中的static目录下，新建一个文件夹native，表示这里放原生小程序编写的组件,放在static里的东西会被直接拷贝到dist/static目录
- 将本库中components下的slider-left文件夹拷贝到native文件夹下
- 在需要使用该组件的页面对应的main.js里面，配置组件名和路径：
![image](./doc-img/demo1.png)
- 在页面中即可通过使用`<slider-left></slider-left>`标签来使用本组件了

ps:  由于mpvue目前对solt scope不支持，所以用mpvue的编写的vue组件是无法在循环中使用组件的，所以这里还是用小程序官方提供的组件编写方式来编写，这样在任何第三方脚手架里均可使用;


## TODO
- [x] `实现原理解析`