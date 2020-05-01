# Chatbot_Web  Chatbot_CN项目的页面UI展示部分

## 功能
提供一个静态的基于 WEB 的用户界面，方便用户和机器人进行对话

## 依赖
python >= 3.5

## 安装
```bash
pip install -r requirements.txt
```

## 启动
```bash
sh start_server.sh
```
访问 http://127.0.0.1:8000 

    调用其他服务的地址在render.py里面修改
    启动服务的端口可以自行指定

## FAQ
1、 为什么我在对话输入框中输入了对话，机器人却不回复我？

答：由于这里的server_url调用的是rasa的restful api服务，所以在和机器人对话之前确保rasa的服务可以正常调用，另外，这个 存在js的跨域请求的问题，一般在浏览器控制台会出现"Access-Control-Allow-Origin"的问题，解决测问题的方法是在启动rasa服务的时候 加上"--cors "*" "参数

## 作者

Xu @ https://github.com/charlesXu86

## Credits
所用的 `webchat.js` 来自于 [rasa-webchat](https://github.com/mrbot-ai/rasa-webchat) 项目

## Resource
本项目参考了 [WeatherBot_UI](https://github.com/howl-anderson/WeatherBot_UI) 项目

## Copyrights

<div>Robot icon in web-chat interface made by <a href="https://www.flaticon.com/authors/good-ware" title="Robotic">Robotic</a> from <a href="https://www.flaticon.com/"     title="Flaticon">www.flaticon.com</a> is licensed by <a href="http://creativecommons.org/licenses/by/3.0/"     title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a></div>
