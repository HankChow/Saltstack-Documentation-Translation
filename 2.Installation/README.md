[原文][1]

# 安装 Salt

本届将会介绍 Salt 的安装方法。如果你是第一次使用 Salt，你需要在一台专用的服务器或者虚拟机上安装 salt-master，然后在需要被 Salt 管理的每个系统上安装 salt-minion。在这个阶段，暂时还不必着重关注整个[系统架构][2]，因为后续可以通过修改配置文件来轻松添加所需的组件，而不需要进行任何重新安装操作。

安装的主要过程包括：

1. 按照适合你所使用的操作系统的安装说明来安装 Salt。你也可以使用 Salt 的<ruby>自动安装<rt>bootstrap</rt></ruby>脚本来进行安装，在这种情况下安装 salt-master 需要加上 `-M` 参数。

2. 确保即将安装 salt-minion 的机器能够[与 salt-master 通信][3]。

3. 在需要被 Salt 管理的每个机器上安装 salt-minion。

4. salt-master 在与 salt-minion 成功通信之后，接受每个 [salt-minion 的密钥][4]。

以上几个步骤完成之后，执行这个命令，就可以接收到所有已连接的 salt-minion 返回的版本信息。

```
salt '*' test.version
```

## 快速安装

在大多数的种类或发行版的操作系统上，都可以使用 [Salt 自动安装脚本][5]安装。

## 特定操作系统的安装指引

以下指引文档介绍如何在各种操作系统上安装 Salt。

* [Arch Linux][5]
* [Debian GNU/Linux / Raspbian][6]
* [Arista EOS Salt minion installation guide][7]
* [Fedora][8]
* [FreeBSD][9]
* [Gentoo][10]
* [OpenBSD][11]
* [macOS][12]
* [RHEL / CentOS / Scientific Linux / Amazon Linux / Oracle Linux][13]
* [Solaris][14]
* [Ubuntu][15]
* [Windows][16]
* [SUSE][17]

# 初始化配置

* [配置 Salt][18]

# 其它相关安装说明

* [Salt 自动安装脚本][19]
* [为 Salt 开放防火墙规则][20]
* [salt-master 服务通信白名单配置][21]
* [使用已被接受的 key 对 salt-minion 进行预配置][22]
* [MacOS(Maverick) 开发者的 Salt 安装说明][23]
* [如何使用普通用户运行 Salt][24]
* [单独运行 salt-minion][25]
* [Salt Masterless 速成教程][26]

# Salt 的依赖项

在满足以下依赖项的前提下，Salt 应该可以在任何类 Unix 操作系统上运行。

* [Python][27]：Python2 >= 2.7，Python3 >= 3.4

* [msgpack-python][28]：高性能的数据交换格式

* [YAML][29]：Python YAML 库

* [Jinja2][30]：解析 salt-states（可以在 salt-master 中配置）

* [MarkupSafe][31] - 在 Python 中安全地处理 XML/HTML/XHTML

* [apache-libcloud][32] - 用于为各种常用云服务提供统一 API 的 Python 库

* [Requests][33] - HTTP 库

* [Tornado][34] - Web 框架、异步网络库

* [futures][35] - 仅 Python2 需要这个依赖项，用于支持 Python 3.2 的并发实现


[1]: https://docs.saltstack.com/en/2019.2/topics/installation/index.html
[2]: /to-be-done.md
[3]: /to-be-done.md
[4]: /to-be-done.md
[5]: /to-be-done.md
[6]: /to-be-done.md
[7]: /to-be-done.md
[8]: /to-be-done.md
[9]: /to-be-done.md
[10]: /to-be-done.md
[11]: /to-be-done.md
[12]: /to-be-done.md
[13]: /to-be-done.md
[14]: /to-be-done.md
[15]: /to-be-done.md
[16]: /to-be-done.md
[17]: /to-be-done.md
[18]: /to-be-done.md
[19]: /to-be-done.md
[20]: /to-be-done.md
[21]: /to-be-done.md
[22]: /to-be-done.md
[23]: /to-be-done.md
[24]: /to-be-done.md
[25]: /to-be-done.md
[26]: /to-be-done.md
[27]: http://python.org/download/
[28]: https://pypi.python.org/pypi/msgpack-python/
[29]: http://pyyaml.org/
[30]: http://jinja.pocoo.org/
[31]: https://pypi.python.org/pypi/MarkupSafe
[32]: http://libcloud.apache.org/
[33]: http://docs.python-requests.org/en/latest
[34]: http://www.tornadoweb.org/en/stable/
[35]: https://github.com/agronholm/pythonfutures
