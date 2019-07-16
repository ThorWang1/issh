# issh
> 自动登录ssh，自动打开端口映射，自动签名debugserver，一键调试，一键shell等等，越狱设备用issh就够了


### Install

> Before install, make sure you have installed iproxy,cfgutil cmds

- `git clone issh_git_project;`
- `cd issh`
- `./install.sh`
- If your shell is bash run: `source ~/.bash_profile` 
- If your shell is zsh run :`source ~/.zshrc`

### Command

- `issh shell`

  get the shell of connect device

- `issh debug [debugArgs:-a pid/processName -x backboard/auto]`

  like `issh debug -a wechat` attach the wechat app

  配合[xia0LLDB](https://github.com/4ch12dy/xia0LLDB)食用更加

- `issh dump [dumpArgs:-l]`

  用的frida-ios-dump脚本，会自动下载并运行

- `issh run "cmd"`

  run shell command on connect idevice like `issh run ls`

- `issh respring/reboot`

  注销和重启设备

- `issh apps`

  显示所有app（包括系统app），包名，显示名，进程名，完整路径等


### Screenshot

![issh-debug](/Users/didi/xia0/shell-script/issh/screenshot/issh-debug.png)



![issh-device](/Users/didi/xia0/shell-script/issh/screenshot/issh-device.png)



![issh-dump](/Users/didi/xia0/shell-script/issh/screenshot/issh-dump.png)



![issh-install](/Users/didi/xia0/shell-script/issh/screenshot/issh-install.png)



![issh-run](/Users/didi/xia0/shell-script/issh/screenshot/issh-run.png)



![issh-scp](/Users/didi/xia0/shell-script/issh/screenshot/issh-scp.png)



![issh-shell](/Users/didi/xia0/shell-script/issh/screenshot/issh-shell.png)



![issh-show-dylib](/Users/didi/xia0/shell-script/issh/screenshot/issh-show-dylib.png)

### Credits

- https://github.com/AloneMonkey/frida-ios-dump
- https://github.com/libimobiledevice/usbmuxd

