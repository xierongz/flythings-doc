---
show_title: false
permalink: /docs/zh/data
key: docs-data-zh
sidebar:
  nav: docs-zh
aside:
  toc: true
layout: article
---
在某些应用场景中需要永久存储一些信息，如存储用户名称、密码或其他配置的一些信息，像这种数据内容比较少的情况，使用数据库去存储，操作起来会很繁琐，这里我们提供了一套简单的数据存储接口，以键-值对的方式存储，接口见storage/StoragePreferences.h：
```c++
// 存储接口
static bool putString(const std::string &key, const std::string &val);
static bool putInt(const std::string &key, int val);
static bool putBool(const std::string &key, bool val);
static bool putFloat(const std::string &key, float val);

// 删除指定键
static bool remove(const std::string &key);
// 清空存储数据
static bool clear();

// 获取接口，获取不到对应键值，返回defVal默认值
static std::string getString(const std::string &key, const std::string &defVal);
static int getInt(const std::string &key, int defVal);
static bool getBool(const std::string &key, bool defVal);
static float getFloat(const std::string &key, float defVal);
```
操作样例：
```c++
// 点击Button1存储用户名，"username":"zkswe"
static bool onButtonClick_Button1(ZKButton *pButton) {
    // 存储用户名
    StoragePreferences::putString("username", "zkswe");
    return false;
}

// 点击Button2获取用户名
static bool onButtonClick_Button2(ZKButton *pButton) {
    // 获取用户名
    std::string username = StoragePreferences::getString("username", "null");
    LOGD("username %s\n", username.c_str());
    return false;
}

// 点击Button3删除用户名
static bool onButtonClick_Button3(ZKButton *pButton) {
    // 删除用户名
    StoragePreferences::remove("username");
    return false;
}
```
