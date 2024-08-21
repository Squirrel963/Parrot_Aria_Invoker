# Parrot Aria Invoker
基于Streamlit库实现的aria2图形化调用工具

其他语言 Other Language：
[English](README.md)

## 配置运行环境
要在您的计算机上运行 PAI，您需要安装 2 个必需的依赖项：
```shell
pip install streamlit
pip install aria2p
```
参考[strymllit官方文档](https://docs.streamlit.io/get-started/installation) 使用命令测试 streamlit：
```shell
streamlit hello
```
下载您需要的 PAI 版本

## 运行
下载完成后，将其解压缩并使用终端打开文件夹，使用以下命令来启动PAI：
```shell
streamlit run PWUI.py
```
或者您可以直接打开文件夹中的***PWUI_starter.bat***文件以启动PAI

## 更改默认设置
您可以通过修改代码的44行~46行来实现更改默认设置，
默认值如下：
```python
44    t_host = st.text_input("host","http://localhost")
45    t_port = st.text_input("port","16800")
46    t_secret = st.text_input("secret key","WfwNk6K8hUpy")
```
假设您的rpc地址为*http://114514.org:1145*
且secret key为*1919810*
您将可以把代码修改为：
```python
44    t_host = st.text_input("host","http://114514.org")
45    t_port = st.text_input("port","1145")
46    t_secret = st.text_input("secret key","1919810")
```

您也可以在图形化面板上直接修改
但是图形化面板的设置仅适合临时使用
因为在您刷新页面后所有设置将会重置为代码中所设置的默认值
