# Parrot Aria Invoker
Graphical aria2 based on the Streamlit lib Invoke the tool

其他语言 Other Language：
[简体中文版本](README_cns.md)

## Configure the runtime environment
To run PAI on your computer, you need to install 2 required dependencies：
```shell
pip install streamlit
pip install aria2p
```
reference[official strymllit documentation](https://docs.streamlit.io/get-started/installation)
Use the command to test streamlit:
```shell
streamlit hello
```
Download the PAI version that you need

## Run
Once the download is complete, unzip it and open the folder using Terminal：
```shell
streamlit run PWUI.py
```
Or you can simply open the ***PWUI_starter.bat*** file in the folder to start PAI

## Change the default settings
You can change the default settings by modifying lines 44~46 of the code , the default values are as follows:
```python
44    t_host = st.text_input("host","http://localhost")
45    t_port = st.text_input("port","16800")
46    t_secret = st.text_input("secret key","WfwNk6K8hUpy")
```
If your RPC address is *http://114514.org:1145*
And the secret key is *1919810*
You can modify the code to:
```python
44    t_host = st.text_input("host","http://114514.org")
45    t_port = st.text_input("port","1145")
46    t_secret = st.text_input("secret key","1919810")
```

You can also modify it directly on the Graphics panel
However, the settings of the graphical panel are only suitable for temporary use
This is because when you refresh the page, all settings will be reset to the defaults set in the code
