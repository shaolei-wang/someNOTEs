## 1. 安装
Terminator最大的特点就是可以在一个窗口中打开多个终端

`sudo apt-get install terminator`

## 2. 快捷键
```
Ctrl+Shift+E    垂直分割窗口
Ctrl+Shift+O    水平分割窗口
    F11         全屏
Ctrl+Shift+C    复制
Ctrl+Shift+V    粘贴
Ctrl+Shift+N    或者 Ctrl+Tab 在分割的各窗口之间切换
Ctrl+Shift+X    将分割的某一个窗口放大至全屏使用
Ctrl+Shift+Z    从放大至全屏的某一窗口回到多窗格界面
```

## 3. 优化配置
初始界面不太美观 
修改配置文件  
 `sudo vim ~/.config/terminator/config`

我的配置如下
```
[global_config]
  geometry_hinting = False
  handle_size = 1
  inactive_color_offset = 1.0
  title_font = mry_KacstQurn Bold 11
  title_hide_sizetext = True
[keybindings]
[layouts]
  [[default]]
    [[[child1]]]
      parent = window0
      profile = default
      type = Terminal
    [[[window0]]]
      parent = ""
      type = Window
[plugins]
[profiles]
  [[default]]
    background_darkness = 0.76
    background_image = None
    background_type = transparent
    cursor_color = "#3036ec"
    custom_command = tmux
    font = Ubuntu Mono 13
    foreground_color = "#ffffff"
    login_shell = True
    show_titlebar = False
    use_system_font = False
```
