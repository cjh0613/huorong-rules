# huorong-rules
![峡州仙士](https://cdn.jsdelivr.net/gh/cjh0613/blog/images/icons/CJHicon.jpg)

[![GitHub stars](https://img.shields.io/github/stars/cjh0613/huorong-rules.svg?style=social)](https://github.com/cjh0613/huorong-rules/stargazers)     [![GitHub forks](https://img.shields.io/github/forks/cjh0613/huorong-rules.svg?style=social)](https://github.com/cjh0613/huorong-rules/network/members)  `Please click on the top right of the page star and fork【请点击页面顶部靠右star与fork】`

[![GitHub release](https://img.shields.io/github/release/cjh0613/huorong-rules.svg?label=%E7%89%88%E6%9C%AC)](https://github.com/cjh0613/huorong-rules/releases/tag/)   ![GitHub top language](https://img.shields.io/github/languages/top/cjh0613/huorong-rules.svg)  ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/cjh0613/huorong-rules.svg)  ![GitHub repo size](https://img.shields.io/github/repo-size/cjh0613/huorong-rules.svg) ![GitHub](https://img.shields.io/github/license/cjh0613/huorong-rules.svg) ![platforms](https://img.shields.io/badge/platform-win32%20%7C%20win64%20%7C%20linux%20%7C%20osx-brightgreen.svg)     [![GitHub issues](https://img.shields.io/github/issues/cjh0613/huorong-rules.svg)](https://github.com/cjh0613/huorong-rules/issues)  [![GitHub closed issues](https://img.shields.io/github/issues-closed/cjh0613/huorong-rules.svg)](https://github.com/cjh0613/huorong-rules/issues?q=is%3Aissue+is%3Aclosed) ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/cjh0613/huorong-rules.svg)   ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/cjh0613/huorong-rules.svg)  ![GitHub contributors](https://img.shields.io/github/contributors/cjh0613/huorong-rules.svg)

## [Donate](https://sponsor.cjh0613.com/index.html) 

## Summary
这个仓库存放我在火绒上使用的，针对腾讯 QQ 的自定义规则。

## 背景

近日，热心网友“mengyx”说，通过火绒安全软件的拦截日志，发现了QQ登录10分钟后会访问存放Edge浏览器历史记录的关键目录。 https://www.v2ex.com/t/745030

另一位网友“qwqdanchun”在看雪论坛上，对此现象进行了进一步分析(点此查看)。根据“qwqdanchun”的分析，该现象不仅仅存在于QQ，还存在于TIM上，它们扫描的也不仅仅是Edge的浏览历史目录，而是会扫描所有基于Chromium引擎的浏览器的浏览历史记录，具体表现为扫描Appdata\Local\下的所有文件夹，然后加上\User Data\Default\History去读取数据。 https://bbs.pediy.com/thread-265359.htm

腾讯在知乎上的官方声明：

```
近日，我们收到外部反馈称PC QQ扫描读取浏览器历史记录。对此，QQ安全团队高度重视并展开调查，发现PC QQ存在读取浏览器历史用以判断用户登录安全风险的情况，读取的数据用于在PC QQ的本地客户端中判断是否恶意登录。所有相关数据不会上传至云端，不会储存，也不会用于任何其他用途。

具体情况为，该操作为历史上线的一个对抗恶意登录的技术解决方案：因系统识别有不少伪造的QQ客户端会恶意访问多个网站作为前期辅助工作，因此在PC QQ客户端中加入了检测恶意和异常的访问逻辑，以此作为辅助手段去判断恶意客户端。

对本次事件，我们深表歉意，内部正梳理历史问题并强化用户数据访问规范。目前，我们已经更换了检测恶意和异常请求的技术逻辑去解决上述安全风险问题，并发布全新的PC QQ版本。为减少不便，所有受影响的PC QQ历史版本将在今天开始进行热更新和推送升级包。同时，手机端QQ不存在上述操作，不受影响。

最后，感谢各位技术爱好者的监督，我们也欢迎大家向腾讯安全应急响应中心（腾讯安全应急响应中心 ）提交报告。
```

腾讯本来就是垄断互联网企业，又闹了这么一出，已经实锤了，既然如此，那就先把腾讯 QQ 给规起来，于是我开辟了这个开源仓库。

If you like this repo, please **click "Star" as support**, thank you!
