- [README 中文](./README-ZH.md)
- [README English](./README.md)

# zmk-config-flkb
FLKB的zmk配置文件，
通过https://nickcoutsos.github.io/keymap-editor/ 来编辑。

## 使用方式

1. Fork 这个存储库.
2. 打开 https://nickcoutsos.github.io/keymap-editor/, 使用你的github账号登陆， 选择你刚刚Fork的存储库, 在图形界面编辑对应的键位映射。
3. 点击保存按钮, GitHub Actions 会自动编译对应的固件。

## 怎么刷入编译好的固件

1. 登陆你自己的github，找到你fork的那个存储库。
2. 点击Actions，然后点击下面的Build。
3. 找到对应修改的Workflow，下载对应的firmware.zip。
4. 解压文件，将键盘通过usb-c连接到电脑，双击键盘背后的reset按钮进入bootloader模式，将left.u2f复制到左边的键盘，right.u2f复制到右边的键盘。
5. 如果右边的键盘没有响应，则同时按下左右的reset按钮同时松开即可。
6. 如果连接不上蓝牙，则可以先下载settings_reset.u2f，分别刷到左右半边，然后再重复4、5两个步骤即可。

参考https://zmk.dev/docs/user-setup
### 现在你的键盘应该可以正常工作了。
