# 使用flask-socketio创建一个网页聊天应用 - Demo 
[视频 | Bilibili](https://www.bilibili.com/video/BV1Rr4y1g7HW/?share_source=copy_web&vd_source=0aaf8e48f5ea3349e83a6332833325be) 

# 安装 / 环境
## requirements.txt 安装
python == 3.10
```bash
pip install requirements.txt
```
## 或者在手动安装
python == 3.10
```cmd
pip install flask==2.0.3
pip install flask_socketio==5.2.0
pip install eventlet==0.33.1
```
因为Werkzeug 3.0. 0已发布，并且Flask没有正确指定依赖项（需求显示Werkzeug>=2.2.0）。所以会出现错误
```cmd
ImportError: cannot import name 'url_quote' from 'werkzeug.urls' (C:\Users\tiany\anaconda3\envs\flask_chat_app\lib\site-packages\werkzeug\urls.py)
```
需安装 2.2.2 版本的Werkzeug
```bash
pip install Werkzeug==2.2.2
```
出现错误 AttributeError: module 'dns.rdtypes' has no attribute 'ANY'
需安装 2.2.1 版本的 dnspython
```bash
pip install dnspython==2.2.1
```

# 注
Flask 实在是太老了bug又多，只适合创建小型项目/网站。需要更高的需求建议更换到 [Django](https://github.com/django/django) 这个项目只作为学习示例。
