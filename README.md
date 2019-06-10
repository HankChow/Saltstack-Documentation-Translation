# Saltstack-Documentation-Translation

本项目针对 [Saltstack 官方文档][1] 进行翻译。由于完工时间不定，因此固定针对 2019.2.0(Fluorine) 版本文档进行翻译。

翻译顺序不严格按照原文档目录的顺序，在项目中已经翻译完成的部分会以指向对应译文页面的超链接表示。

本项目维护一份[术语表][2]，文档中出现频率较高的一些固定译法会记录在术语表当中。


## 文档目录

* [Salt 简介(Introduction to Salt)][3]
  * [30 秒搞懂 Salt 是什么(The 30 second summary)][4]
  * [简洁(Simplicity)][5]
  * [并发操作(Parallel execution)][6]
  * [建立在成熟可靠的技术基础上(Builds on proven technology)][7]
  * [Python 客户端接口(Python client interface)][8]
  * [快速、灵活、可扩展(Fast, flexible, scalable)][9]
  * [开源(Open)][10]
  * [Salt 社区(Salt Community)][11]
  * [邮件列表(Mailing List)][12]
  * [IRC][13]
  * [在 GitHub 上关注 Salt(Follow on Github)][14]
  * [博客(Blogs)][15]
  * [Salt states 样例(Example Salt States)][16]
  * [在 OpenHub 上关注 Salt(Follow on Open Hub)][17]
  * [相关社区链接(Other community links)][18]
  * [为 Salt 贡献代码(Hack the Source)][19]
* [Installation][20]
  * [Quick Install][21]
  * [Platform-specific Installation Instructions][22]
  * [Initial Configuration][23]
  * [Additional Installation Guides][24]
  * [Dependencies][25]
  * [Optional Dependencies][26]
  * [Upgrading Salt][27]
  * [Building Packages using Salt Pack][28]
* Configuring Salt
  * Configuring the Salt Master
  * Configuring the Salt Minion
  * Configuring the Salt Proxy Minion
  * Configuration file examples
  * Minion Blackout Configuration
  * Access Control System
  * Job Management
  * Managing the Job Cache
  * Storing Job Results in an External System
  * Logging
  * External Logging Handlers
  * salt.log.handlers.fluent_mod
  * salt.log.handlers.log4mongo_mod
  * salt.log.handlers.logstash_mod
  * salt.log.handlers.sentry_mod
  * Salt File Server
  * Git Fileserver Backend Walkthrough
  * MinionFS Backend Walkthrough
  * Salt Package Manager
  * Storing Data in Other Databases
  * Running the Salt Master/Minion as an Unprivileged User
  * Using cron with Salt
  * Use cron to initiate a highstate
  * Hardening Salt
  * Security disclosure policy
  * Salt Transport
  * Master Tops System
  * Returners
  * Renderers
* Using Salt
  * Grains
  * Storing Static Data in the Pillar
  * Targeting Minions
  * The Salt Mine
  * Runners
  * Salt Engines
  * Understanding YAML
  * Understanding Jinja
  * Tutorials Index
  * Troubleshooting
  * Frequently Asked Questions
  * Salt Best Practices
* Remote Execution
  * Remote execution tutorial
  * Running Commands on Salt Minions
  * Writing Execution Modules
  * Executors
* Configuration Management
  * How Do I Use Salt States?
  * States tutorial, part 1 - Basic Usage
  * States tutorial, part 2 - More Complex States, Requisites
  * States tutorial, part 3 - Templating, Includes, Extends
  * States tutorial, part 4
  * State System Reference
* Return Codes
  * Retcode Passthrough
* Utility Modules - Code Reuse in Custom Modules
* Events & Reactor
  * Event System
  * Beacons
  * Reactor System
* Orchestration
  * Orchestrate Runner
* Solaris
  * Solaris-specific Behaviour
* Salt SSH
  * Getting Started
  * Salt SSH Roster
  * Deploy ssh key for salt-ssh
  * Calling Salt SSH
  * States Via Salt SSH
  * Targeting with Salt SSH
  * Configuring Salt SSH
  * Running Salt SSH as non-root user
  * Define CLI Options with Saltfile
  * Debugging salt-ssh
* Thorium Complex Reactor
  * Starting the Thorium Engine
  * Thorium Modules
  * Writing Thorium Formulas
  * The Thorium Register
* Salt Cloud
  * Configuration
  * Configuration Inheritance
  * QuickStart
  * Using Salt Cloud
  * Core Configuration
  * Windows Configuration
  * Cloud Provider Specifics
  * Miscellaneous Options
  * Troubleshooting Steps
  * Extending Salt Cloud
  * Using Salt Cloud from Salt
  * Feature Comparison
  * Tutorials
* Salt Proxy Minion
  * New in 2017.7.0
  * New in 2016.11.0
  * New in 2016.3
  * New in 2015.8.2
  * New in 2015.8
  * Getting Started
  * The __proxyenabled__ directive
  * SSH Proxymodules
* Network Automation
  * New in Carbon (2016.11)
  * NAPALM
  * JUNOS
* Salt Virt
  * Salt Virt Tutorial
  * The Salt Virt Runner
  * Based on Live State Data
  * Deploy from Network or Disk
* Command Line Reference
  * salt-call
  * salt
  * salt-cloud
  * salt-cp
  * salt-extend
  * salt-key
  * salt-master
  * salt-minion
  * salt-proxy
  * salt-run
  * salt-ssh
  * salt-syndic
  * salt-unity
  * salt-api
  * spm
* Pillars
* Master Tops
* Salt Module Reference
  * auth modules
  * beacon modules
  * Cache Modules
  * cloud modules
  * engine modules
  * executors modules
  * fileserver modules
  * grains modules
  * execution modules
  * netapi modules
  * output modules
  * pillar modules
  * proxy modules
  * queue modules
  * renderer modules
  * returner modules
  * roster modules
  * runner modules
  * sdb modules
  * serializer modules
  * state modules
  * thorium modules
  * master tops modules
  * wheel modules
* APIs
  * Python client API
  * netapi modules
* Architecture
  * High Availability Features in Salt
  * Salt Syndic
  * Using Salt at scale
  * Multi Master Tutorial
  * Multi-Master-PKI Tutorial With Failover
* Minion Data Cache
  * Pluggable Data Cache
  * Configuring the Minion Data Cache
* Slots
  * Execution functions
* Windows
  * Windows Software Repository
  * Windows-specific Behaviour
* Developing Salt
  * Overview
  * Salt Client
  * Salt Master
  * Salt Minion
  * A Note on ClearFuncs vs. AESFuncs
  * Contributing
  * Deprecating Code
  * Installing Salt for development
  * GitHub Labels and Milestones
  * Logging Internals
  * Package Providers
  * Pull Requests
  * Reporting Bugs
  * Salt Topology
  * Translating Documentation
  * Developing Salt Tutorial
  * Modular Systems
  * Salt Extend
  * Salt's Test Suite
  * Integration Tests
  * Writing Unit Tests
  * raet
  * SaltStack Git Policy
  * Salt Conventions
  * Salt code and internals
  * Salt Community Projects
  * Salt's Test Suite: An Introduction
* Release Notes
  * Latest Branch Release
  * Previous Releases
* Venafi Tools for Salt
  * Introduction
  * Example Usage
  * Runner Functions
* Glossary


[1]: https://docs.saltstack.com/en/2019.2/contents.html
[2]: glossary.md
[3]: 1.Introduction%20to%20Salt#salt-%E7%AE%80%E4%BB%8B
[4]: 1.Introduction%20to%20Salt#30-%E7%A7%92%E6%90%9E%E6%87%82-salt-%E6%98%AF%E4%BB%80%E4%B9%88
[5]: 1.Introduction%20to%20Salt#%E7%AE%80%E6%B4%81
[6]: 1.Introduction%20to%20Salt#%E5%B9%B6%E5%8F%91%E6%93%8D%E4%BD%9C
[7]: 1.Introduction%20to%20Salt#%E5%BB%BA%E7%AB%8B%E5%9C%A8%E6%88%90%E7%86%9F%E5%8F%AF%E9%9D%A0%E7%9A%84%E6%8A%80%E6%9C%AF%E5%9F%BA%E7%A1%80%E4%B8%8A
[8]: 1.Introduction%20to%20Salt#python-%E5%AE%A2%E6%88%B7%E7%AB%AF%E6%8E%A5%E5%8F%A3
[9]: 1.Introduction%20to%20Salt#%E5%BF%AB%E9%80%9F%E7%81%B5%E6%B4%BB%E5%8F%AF%E6%89%A9%E5%B1%95
[10]: 1.Introduction%20to%20Salt#%E5%BC%80%E6%BA%90
[11]: 1.Introduction%20to%20Salt#salt-%E7%A4%BE%E5%8C%BA
[12]: 1.Introduction%20to%20Salt#%E9%82%AE%E4%BB%B6%E5%88%97%E8%A1%A8
[13]: 1.Introduction%20to%20Salt#irc
[14]: 1.Introduction%20to%20Salt#%E5%9C%A8-github-%E4%B8%8A%E5%85%B3%E6%B3%A8-salt
[15]: 1.Introduction%20to%20Salt#%E5%8D%9A%E5%AE%A2
[16]: 1.Introduction%20to%20Salt#salt-states-%E6%A0%B7%E4%BE%8B
[17]: 1.Introduction%20to%20Salt#%E5%9C%A8-openhub-%E4%B8%8A%E5%85%B3%E6%B3%A8-salt
[18]: 1.Introduction%20to%20Salt#%E7%9B%B8%E5%85%B3%E7%A4%BE%E5%8C%BA%E9%93%BE%E6%8E%A5
[19]: 1.Introduction%20to%20Salt#%E4%B8%BA-salt-%E8%B4%A1%E7%8C%AE%E4%BB%A3%E7%A0%81
[20]: 2.Installation#%E5%AE%89%E8%A3%85-salt
[21]: 2.Installation#%E5%BF%AB%E9%80%9F%E5%AE%89%E8%A3%85
[22]: 2.Installation#%E7%89%B9%E5%AE%9A%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F%E7%9A%84%E5%AE%89%E8%A3%85%E6%8C%87%E5%BC%95
[23]: 2.Installation#%E5%88%9D%E5%A7%8B%E5%8C%96%E9%85%8D%E7%BD%AE
[24]: 2.Installation#%E5%85%B6%E5%AE%83%E7%9B%B8%E5%85%B3%E5%AE%89%E8%A3%85%E8%AF%B4%E6%98%8E
[25]: 2.Installation#salt-%E7%9A%84%E4%BE%9D%E8%B5%96%E9%A1%B9 
[26]: 2.Installation#%E5%8F%AF%E9%80%89%E4%BE%9D%E8%B5%96%E9%A1%B9
[27]: 2.Installation#%E5%8D%87%E7%BA%A7-salt
[28]: 2.Installation#%E4%BD%BF%E7%94%A8-salt-pack-%E6%9E%84%E5%BB%BA%E8%BD%AF%E4%BB%B6%E5%8C%85 
