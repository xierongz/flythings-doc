---
show_title: false
permalink: /docs/zh/window
key: docs-window-zh
sidebar:
  nav: docs-zh
aside:
  toc: true
layout: article
---

# 窗口
## 功能描述
窗口实际是一个容器部件。可以包含所有的控件，也可以再次包含一个新的窗口。可以用于以下场景
* 显示隐藏一个控件组合
* 当需要完成tab页面的时候可以通过多个窗口实现不同的窗口切换
* 弹出的对话框
* 弹出悬浮框

## 如何使用  
1. 创建一个 **窗口** 控件，默认的窗口是透明的。根据需求，可以自行添加背景图或者修改背景色；  你也可以将其他控件添加到窗口中。  

   ![](assets/window/properties.png)
2. 在上面的属性表中 有两个属性需要解释下:  
  * **是否是模态窗口**  
    如果是模态，当这个窗口控件显示时，点击该窗口以外的区域，该窗口会自动隐藏。  
    如果是非模态， 该窗口控件的显示/隐藏 都必须自行控制。
  * 超时自动隐藏窗口  
    如果是模态窗口， 那么该窗口从刚开始显示开始计时，在指定时间后自动隐藏。单位为秒；如果该值为 -1，那么表示不会自动隐藏。  
    如果是非模态，那么该参数无任何作用。

## 代码操作  
对于窗口控件，我们一般会涉及到如下几个函数  
```
//显示窗口
void showWnd();
//隐藏窗口
void hideWnd();
判断窗口是否显示
bool isWndShow();
```
# 样例代码
演示了 模态/非模态窗口控件的使用  

![](assets/window/preview.png) 

具体窗口控件的使用，参考[样例代码](demo_download#demo_download)  
