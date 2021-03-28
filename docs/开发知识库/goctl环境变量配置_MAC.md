go-zero官方资料中对于goctl的环境配置没有明确的提示，收集整理了资料供大家参考<br />MacOS 11.2.3<br />
<br />1、打开或者创建 shell 的 `rc` 文件，比如，在 Linux 和 macOS Mojave 或 Mojave 之前的系统里，是默认使用 Bash 的，所以需要修改 `$HOME/.bashrc` 文件。 macOS Catalina 操作系统默认使用 Z Shell，所以需要修改 `$HOME/.zshrc` 文件。请知晓，如果你使用不同的 shell，文件目录或文件名可能会有所不同。

通过一下命令用文本编辑器打开 .bash_profile文件
```bash
open -e ~/.bash_profile
```


2、在文件中增加下列这行代码，注意：将其中的[Users/guangsi/go/bin]路径更改为你本机go的安装路径：
```bash
export PATH=/Users/guangsi/go/bin:$PATH
```
保存并关闭文本编辑器<br />
<br />3、运行 `source $HOME/.bash_profile` 来刷新当前命令行窗口。
```bash
source $HOME/.bash_profile
```
4、通过运行以下命令来验证 文件夹是否已经添加到 PATH 环境变量中：
```bash
 echo $PATH
```
5、验证命令是否可用，可以执行下面的命令检测：
```bash
 which goctl
```
出现以下结果，表明已经安装成功
```bash
/Users/guangsi/go/bin/goctl
```


