---
show_title: false
permalink: /docs/zh/editor_tip
key: docs-editor_tip-zh
sidebar:
  nav: docs-zh
aside:
  toc: true
layout: article
---
# 开发工具常用设置

## <span id = "jump_to_source"> 快速跳转至关联函数</span>
当我们在UI文件中添加了过多的控件时，**Logic.cc**文件中也会生成多个关联函数。如果想要查找某个控件的关联函数是相当费时的事。  
好在工具提供了一个从UI控件 **快速跳转至相关代码** 的功能。  
在预览图上，选中一个控件，右键，在弹出菜单中选择 **跳转到相关代码**，即可打开对应的Logic.cc文件，并且会将光标定位到该控件的关联函数的位置。  

   ![](assets/ide/jump_to_source.png)

> **注意：该功能仅对会自动生成关联函数的控件类型有效，比如上文中提到的控件类型，如果你选择的是其他控件类型，那么功能只会跳转到相对应的Logic.cc文件，并将光标定位于文件底部。**
   
   
---     

## 修改字体/字体大小  
1. 在工具的菜单栏上， 选择 **窗口** -> **首选项**      

      ![](assets/ide/preference.png)

2.  在弹出框中， 依次按照下图选择，即可设置字体。    
  
     ![](assets/ide/set_font.png)

## 代码智能补全  
编辑代码时，先需要输入起始部分，然后键入 **Alt + /** 可以打开代码补全功能。   
如下图， 我输入的 **UA** 两个字母， 然后键入 **Alt + /** 快捷键， 可以看到给出了多个补全选项， 用上下方向键可以进行选择。**Enter**键确认选择。  

  ![](assets/ide/intelisence.png)
  

## 重建索引  
 如果出现代码补全功能失效，或者编辑器提示代码错误，但是编译却没有问题的情况，请尝试重建索引。  
 
 重建索引的步骤如下：   
 
 ![](assets/ide/rebuild_index.gif)  
