# CrawleeAwesome

# 工具链
对于Crawlee-Python爬虫开发，推荐工具链选择如下：
💡 首推 VS Code + Python扩展

✅ 轻量高效：启动速度快，插件生态丰富（Python/Pylance/Jupyter等扩展完美支持爬虫开发）
✅ 调试利器：可视化调试器对爬虫的请求响应调试特别友好，支持XPath/CSS选择器实时测试
✅ 虚拟环境整合：通过终端面板直接管理conda/venv虚拟环境，适配Crawlee等框架的依赖管理

VS 2022的适用场景
若需同时开发C#/.NET混合项目，可用其Python环境功能，但注意：
⚠️ 相较于VS Code，在纯Python开发中会占用更多系统资源
⚠️ 部分Python插件功能（如Jupyter notebook交互）不如VS Code流畅
✨ 开发小技巧
使用pipenv创建独立环境，搭配VS Code的Python扩展自动识别虚拟环境，能有效避免依赖冲突：
bash复制pipenv install crawlee camoufox 

# 文章
Crawlee-Python项目环境配置与安装指南
https://blog.csdn.net/gitblog_00243/article/details/148490803
