# CrawleeAwesome
从成熟度和功能完整性来看，Crawlee 的 JavaScript/TypeScript 版本（JS/TS）比 Python 版本更完善。JS/TS 版本作为 Crawlee 的原始实现，已积累超过 15k GitHub 星标，提供了完整的爬虫生态，包括 <code>CheerioCrawler</code>、<code>PuppeteerCrawler</code> 和 <code>PlaywrightCrawler</code> 三大核心类，支持 HTTP 请求、无头浏览器渲染、反检测机制（如代理轮换、浏览器指纹）以及自动扩展功能。其 API 设计稳定，文档丰富，且与 Node.js 生态无缝集成，可直接调用 Puppeteer 或 Playwright 进行复杂的浏览器自动化操作。

相比之下，Python 版本目前处于「早期采用者」阶段，尽管在 GitHub 上发布后一周内就获得 3.1k 星标，但功能覆盖和社区支持仍在追赶中。虽然它继承了核心反阻塞能力（如默认配置下模拟人类行为避开检测），但工具链生态尚未完全成熟，例如文档示例和第三方库集成不如 JS/TS 版本全面。不过，Python 版本的优势在于依托 Python 在数据科学领域的流行度，适合熟悉该语言的开发者快速上手网络数据采集。

选择时可遵循「技术栈匹配」原则：若团队擅长 Node.js/TypeScript 或需要构建复杂的浏览器自动化爬虫，优先选择 JS/TS 版本；若项目依赖 Python 数据处理工具链（如 Pandas、Scrapy），可尝试 Python 版本，但需注意其仍在快速迭代中，部分高级功能可能尚未稳定。随着 Python 版本的持续开发（如近期新增文件下载功能），两者的差距可能逐步缩小，但就当前（2025 年）而言，JS/TS 版本仍是更可靠的选择。

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

Camoufox项目中WebGL启用问题的技术解析
https://blog.gitcode.com/69b4296135dfafc6dd552aca5c74f3c2.html

使用 Crawlee 下载文件
https://www.studywithgpt.com/zh-cn/tutorial/tf4ez7

使用 Crawlee 进行网页抓取 – 分步指南
https://www.bright.cn/blog/web-data/web-scraping-with-crawlee

我用 crawlee 抓取了 9 月掘金所有面试相关文章
https://juejin.cn/post/7425626637816954943

Camoufox项目中实现网络请求拦截的技术解析
https://blog.gitcode.com/ab215d0a960f8daecce95e47ce3aa22e.html

使用Crawlee爬取 豆瓣电影 Top 250 的数据
https://www.juetan.cn/tools/crawlee/

使用Crawlee进行代理管理
https://www.studywithgpt.com/zh-cn/tutorial/up5epe

爬取整个示例商店并找到所有数据，首先需要访问所有产品页面-浏览所有可用分类以及所有产品详细页。
https://bannermiao.github.io/crawlee-cn/docs/introduction/crawling

深入解析Apify Crawlee-Python中的Playwright爬虫浏览器配置
https://blog.csdn.net/gitblog_00737/article/details/148490782

# Camoufox
Camoufox项目中Playwright连接Firefox浏览器的正确方式解析
https://blog.gitcode.com/d2b72de2b14b270e8cf29e28ac947492.html

Camoufox项目：多用户目录配置实现浏览器多实例隔离
https://blog.gitcode.com/1bb69228735c2ff74e336fd5932e637f.html

Camoufox项目中的浏览器缓存机制优化实践
https://blog.gitcode.com/d4366b3810f1949c585a9dec70ace575.html

Camoufox项目中GeoIP功能异步调用问题的分析与修复
https://blog.gitcode.com/9718016b09beba962b8742af33079490.html

