[原文](https://docs.saltstack.com/en/2019.2/topics/index.html)

# Salt 简介

> 本文档不是讨论氯化钠（NaCl）的文档。

## 30 秒搞懂 Salt 是什么

Salt 是：

* 一个配置管理系统，可以将远程节点维护在一个所需的的状态（例如让远程节点安装指定的软件包、运行指定的服务）

* 一个分布式的远程执行系统，可以通过多种形式选择远程节点执行命令和查询数据

为了将远程执行过程中的最佳方案结合到一起，并让这个过程变得更快、更稳定、更具可扩展性，Salt 因此而诞生了。Salt 简单易管理的界面不仅可以让你管理数十台乃至数千台服务器，更能让你快速处理大量信息。

## 简洁

在大规模部署和小型系统之间提供多功能性，这样的任务似乎令人望而生畏，但如果使用 Salt，其中的设置和维护工作就会变得非常简单。Salt 的架构适用于任意数量的服务器，无论项目的规模是从本地网络的少数系统还是跨数据中心的全球级部署。Salt 是一个简单的服务器/客户机拓扑模型，并将所需的功能内置在守护进程当中。虽然 Salt 的默认配置几乎不需要修改就可以使用，但也可以通过微调来满足特定的需求。

## 并发操作

Salt 的核心功能包括：

* 能够并行地让管理命令在多个远程系统中同时执行，避免低效的串行执行

* 使用安全加密的传输协议

* 尽可能减轻网络负载

* 提供简洁的编程接口

Salt 还可以更精细地控制远程执行操作，除了主机名之外，还支持按照系统属性来选择远程执行的目标系统。

## 建立在成熟可靠的技术基础上

Salt 采用了多种技术。在网络层使用了优秀的 ZeroMQ 网络库，因此 Salt 守护进程包含了一个可用且透明的 AMQ 代理。身份验证和加密是 Salt 运行的重要一环，因此 Salt 主守护进程通过公钥进行身份验证，然后使用更快的 AES 算法对负载通信进行加密。Salt 还使用了 msgpack 数据编码格式进行通信，以实现快速轻量的网络负载。

## Python 客户端接口

为实现一些简单的扩展，可以将 Salt 执行过程编写成普通的 Python 模块。通过 Salt 执行命令收集到的数据可以发回主服务器，也可以发送到其它任意程序。你可以使用简单的 Python API 调用 Salt，也可以在命令行调用 Salt。因此 Salt 不仅可以用于执行一些一次性的命令，还可以作为大型程序的一个组成部分。

## 快速、灵活、可扩展

Salt 是一个可以从一台服务器上控制多台服务器快速执行命令的系统，它具有快速、易配置、可扩展的特点，同时还提供了一个单一的远程执行体系结构，以满足管理任意数量的服务器的需求。Salt 的基础架构中汇集了远程执行方面的很多最佳实践，在此基础上又进一步扩展了它的功能，最终形成了 Salt 这样一个实用性和普适性都很强的系统。

## 开源

Salt 在 [Apache 2.0 许可](http://www.apache.org/licenses/LICENSE-2.0.html) 下开发，可以在开源或私有项目中使用。欢迎你将你的功能扩展代码提交到 Salt 项目，让我们与 Salt 共同成长、共同受益。

## Salt 社区

欢迎加入 Salt！

你可以通过很多途径参与 Salt 社区的交流，例如 IRC 频道、邮件列表等等。

## 邮件列表

[salt-user 邮件列表](https://groups.google.com/forum/#!forum/salt-users) 是关注 Salt 最新问题和进展的最好的地方，欢迎加入。这个邮件列表由 Google Groups 托管，并且对新成员开放。

## IRC

`#salt` IRC 频道在 [Freenode](http://freenode.net/irc_servers.shtml) 上托管，在浏览器里通过 [Freenode 聊天客户端](http://webchat.freenode.net/?channels=salt&uio=Mj10cnVlJjk9dHJ1ZSYxMD10cnVl83) 即可访问。

Moritz Lenz 正在收集 [IRC 频道活动的日志](http://irclog.perlgeek.de/salt/)。

如果你对 Salt 的开发感兴趣，欢迎加入 `#salt-devel` 频道参与讨论。

## 在 GitHub 上关注 Salt

Salt 的源代码托管在 Github 上，关注这个项目，可以获取项目的更新信息以及相关事项。

GitHub 地址：[http://www.saltstack.com/blog/](http://www.saltstack.com/blog/)

## 博客

SaltStack 公司会在 [博客](http://www.saltstack.com/blog/) 中发布最近的新闻和项目进展。

博客地址：[http://www.saltstack.com/blog/](http://www.saltstack.com/blog/)

## Salt states 样例

官方 `salt-states` 的 GitHub 仓库地址：[https://github.com/saltstack/salt-states](https://github.com/saltstack/salt-states)

以下是一些由社区提供的 salt states 样例：

* [https://github.com/blast-hardcheese/blast-salt-states](https://github.com/blast-hardcheese/blast-salt-states)

* [https://github.com/kevingranade/kevingranade-salt-state](https://github.com/kevingranade/kevingranade-salt-state)

* [https://github.com/uggedal/states](https://github.com/uggedal/states)

* [https://github.com/mattmcclean/salt-openstack/tree/master/salt](https://github.com/mattmcclean/salt-openstack/tree/master/salt)

* [https://github.com/rentalita/ubuntu-setup/](https://github.com/rentalita/ubuntu-setup/)

* [https://github.com/brutasse/states](https://github.com/brutasse/states)

* [https://github.com/bclermont/states](https://github.com/bclermont/states)

* [https://github.com/pcrews/salt-data](https://github.com/pcrews/salt-data)


## 在 OpenHub 上关注 Salt

[https://www.openhub.net/p/salt](https://www.openhub.net/p/salt)

## 相关社区链接

* [Salt Stack Inc.](http://www.saltstack.com/)

* [Subreddit](http://www.reddit.com/r/saltstack)

* [Google+](https://plus.google.com/114449193225626631691/posts)

* [YouTube](http://www.youtube.com/user/SaltStack)

* [Facebook](https://www.facebook.com/SaltStack)

* [Twitter](https://twitter.com/SaltStackInc)

* [Wikipedia page](http://en.wikipedia.org/wiki/Salt_(software))

* [Stack Overflow](https://stackoverflow.com/questions/tagged/salt-stack)

## 为 Salt 贡献代码

如果你希望为 Salt 的代码和文档作出贡献，请参阅 [贡献文档](https://docs.saltstack.com/en/2019.2/topics/development/contributing.html#contributing)。
