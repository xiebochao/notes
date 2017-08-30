## 在 Ubuntu 下安装 Wing IDE
1. 下载 Wing IDE Personal
2. 安装依赖 enscript
```
sudo apt-get install enscript
```
3. 定位到安装包所在位置后
```
sudo dpkg -i wingide5_5.1.11-1_amd64.deb
```
## 更换主题
`Edit`-`Preference`-`User Interface`
## 安装Python 3 并在 Wing IDE 下切换 Python 版本
> Ubuntu 中自带 Python，但课上使用 Python 3
1. 安装 Python 3 和 pip 3
```
sudo apt-get install python3
sudo apt-get install python3-pip
```
2. 安装后通过以下命令可以查看到 Python 3 的版本号，证明安装成功
```
python 3 -V
```
3. 通过以下命令可以查看 Python 3 的安装位置
```
which python3
```
4. 在 Wing IDE 中：`Source`-`Show Python Environment...`，单击`Change Settings`，修改 Python Executable 和 Python Path 即可
