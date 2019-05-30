[原文][1]

# 安装 Salt

本届将会介绍 Salt 的安装方法。如果你是第一次使用 Salt，你需要在一台专用的服务器或者虚拟机上安装 salt-master，然后在需要被 Salt 管理的每个系统上安装 salt-minion。在这个阶段，暂时还不必着重关注整个[系统架构][2]，因为后续可以通过修改配置文件来轻松添加所需的组件，而不需要进行任何重新安装操作。

安装的主要过程包括：

1. 按照适合你所使用的操作系统的安装说明来安装 Salt。你也可以说通过运行 Salt 的<ruby>自动安装<rt>bootstrap</rt></ruby>脚本来进行安装，在这种情况下安装 salt-master 需要加上 `-M` 参数。

2. 确保即将安装 salt-minion 的机器能够[与 salt-master 通信][3]。

3. 在需要被 Salt 管理的每个机器上安装 salt-minion。

4. salt-master 在与 salt-minion 成功通信之后，接受每个 [salt-minion 的密钥][4]。

以上几个步骤完成之后，执行这个命令，就可以接收到所有已连接的 salt-minion 返回的版本信息。

```
salt '*' test.version
```

## 快速安装


[1]: https://docs.saltstack.com/en/2019.2/topics/installation/index.html
[2]: /to-be-done.md
[3]: /to-be-done.md
[4]: /to-be-done.md
