# Crawlee
Crawlee for Python
https://github.com/apify/crawlee-python
Crawlee for JS/TS
https://github.com/apify/crawlee

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
Crawlee + Playwright + Camoufox
https://apify.com/templates/js-crawlee-playwright-camoufox

如果你想尽快尝试一下，那么你可以检查这个分支：
https://github.com/apify/crawlee-python/tree/camoufox
如果你从那个分支运行这个playwright_crawler_example，那么它将使用 camoufox。
https://github.com/apify/crawlee-python/issues/684

Crawlee 快速开始
https://bannermiao.github.io/crawlee-cn/docs/quick-start

演示如何使用 PlaywrightCrawler 使用无头 Chromium 和 Playwright 递归抓取 Hacker 新闻网站。
https://crawlee.dev/python/docs/examples/playwright-crawler
具有阻止请求的剧作家爬虫
https://crawlee.dev/python/docs/examples/playwright-crawler-with-block-requests

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

Crawlee-Python项目：处理大规模爬取任务失败的最佳实践
https://blog.gitcode.com/e5a6071685108d4ee83c61a9869f037b.html

Crawlee项目在Windows开发与AWS部署中的浏览器版本不匹配问题解析
https://blog.gitcode.com/c1bed13121206e68549c698e17b472ad.html

crawlee自动网页抓取和浏览第一篇
https://blog.csdn.net/qingyou2006/article/details/129611568

[Crawlee项目中的Cookie设置URL解析问题解析](https://blog.gitcode.com/ae8f2c69c4e5e36e53870587687171bf.html)

[如何为 Crawlee 设置代理](https://proxy-port.com/zh-hans/how-to/set-up-proxy-for-crawlee)

[在Crawlee中添加数据到数据集](https://www.studywithgpt.com/zh-cn/tutorial/nabtq6)

[深入Crawlee架构：从基础爬虫到高级功能](https://blog.csdn.net/gitblog_01129/article/details/148490790)

# Crawlee-Python
[Crawlee for Python 替代品](https://www.aibase.com/zh/tool/31600)

Crawlee-Python项目：实现持续运行的网络爬虫循环
https://blog.gitcode.com/9d65c6325880a3a0b8a279b4931ff7b7.html

Crawlee-Python项目环境配置与安装指南
https://blog.csdn.net/gitblog_00243/article/details/148490803

Crawlee-Python项目中的PlaywrightCrawler指纹生成机制优化
https://blog.gitcode.com/10612aaf4204d58a90bd66af1cfe6582.html

Crawlee-Python v0.5.4版本发布：浏览器隐私模式支持与关键修复
https://blog.gitcode.com/adcbc244245aebee2701cc15a6469daa.html

Crawlee-Python爬虫模板系统：快速生成项目结构
https://blog.csdn.net/gitblog_00643/article/details/151321665

[Crawlee-Python CLI工具使用体验优化指南](https://blog.gitcode.com/1970157308c88f8dd28c03d1f5a6fcb7.html)

[Crawlee-Python项目中的Configuration类优化实践](https://blog.gitcode.com/2a224d29f1395b550469c367ef43a998.html)

# Camoufox
[🦊 反检测浏览器](https://github.com/daijro/)

一个功能强大的 CLI 工具，用于抓取网站和下载内容，包括 HTML、图像和视频。Web Grabber 提供多种浏览模式，包括正常请求、用于 JavaScript 渲染的 Selenium 和用于反机器人保护的 camoufox。
完整的网站抓取：从网站下载所有 HTML 页面、图像和视频
交互模式：选择保存路径补全内容的位置
自动目录命名：自动创建以网站域命名的目录
反机器人保护：使用伪装来避免被反机器人机制检测到
Tor 集成：通过 Tor 网络路由流量以实现匿名
Selenium 支持：为动态网站渲染 JavaScript -- Chrome/Chromium（用于 Selenium 和 camoufox 模式）
多线程下载：高效并行下载资源
有针对性的抓取：使用 CSS 选择器提取特定元素
https://github.com/tadeasf/web-grabber

为 Playwright 自动解决验证码。支持 Cloudflare Turnstile 和 Interstitial，以及具有基于点击或 API （2captcha） 解决的 reCAPTCHA V2 和 V3。专为与 Playwright、Patchright 和 Camoufox 轻松集成而设计。
https://github.com/techinz/playwright-captcha

[轻量级 camoufox-js 替代方案，仅导出“launchOptions”，旨在与 Playwright 一起使用](https://github.com/CyborgDragonFire/camoufox-launchOptions)

[带有 Camoufox 的Playwright爬虫](https://crawlee.dev/python/docs/examples/playwright-crawler-with-camoufox)

[CamouFox项目中连接与位置检测警告的优化实践](https://blog.gitcode.com/c837d7f96e21c24d5f063f01239945ae.html)

[Camoufox项目中WebGL启用问题的技术解析](https://blog.gitcode.com/69b4296135dfafc6dd552aca5c74f3c2.html)

[Crawlee-Python 整合 Camoufox 实现高级反检测爬虫](https://blog.gitcode.com/a054a2c1740ebb73be247308392bb1b2.html)

无头 Firefox 抓取工具使用 Camoufox 进行隐身，使用 Playwright 进行浏览器自动化。
配置为使用 Docker 在 Railway 上部署。
https://github.com/railtools/camoufox-py

Camoufox项目中的Firefox无头模式检测与绕过技术分析
https://blog.gitcode.com/40322473eb7a9a735959e720baa1f448.html

Camoufox项目中Playwright连接Firefox浏览器的正确方式解析
https://blog.gitcode.com/d2b72de2b14b270e8cf29e28ac947492.html

Camoufox项目：多用户目录配置实现浏览器多实例隔离
https://blog.gitcode.com/1bb69228735c2ff74e336fd5932e637f.html

Camoufox项目中的浏览器缓存机制优化实践
https://blog.gitcode.com/d4366b3810f1949c585a9dec70ace575.html

Camoufox项目中GeoIP功能异步调用问题的分析与修复
https://blog.gitcode.com/9718016b09beba962b8742af33079490.html

Camoufox项目中浏览器窗口尺寸控制的正确方法
https://blog.gitcode.com/6d8dfae67915f5fb54ba450ca8151bd1.html

CamouFox项目中的Canvas指纹防护技术演进
https://blog.gitcode.com/43976cf7adc0204d8d263075bb7c3876.html

Camoufox：隐匿的网络爬取利器
https://blog.csdn.net/gitblog_00782/article/details/146532749

Camoufox项目中元素边界框获取超时问题解析
https://blog.gitcode.com/97b3156785a5a494e2c3604e3b84cadf.html

在Docker容器中运行Camoufox反检测浏览器的技术实践
https://blog.gitcode.com/f1124ebcb1f9018d0c3bb082506c5bfb.html

# Cloudflare
2025年如何绕过Cloudflare反爬虫挑战 Cloudflare是爬虫的克星
https://www.capsolver.com/zh/blog/All/bypass-cloudflare-challenge-2025

如何在 2025 年使用 Playwright 绕过 Cloudflare
方法 1：使用 Stealth 插件
方法 2：使用代理
方法 3：解决验证码
方法 4：使用 ZenRows 绕过高级 Cloudflare 保护
https://www.zenrows.com/blog/playwright-cloudflare-bypass

绕过 Cloudflare：最佳实践
https://github.com/bright-cn/bypass-cloudflare
