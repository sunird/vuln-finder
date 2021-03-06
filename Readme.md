### vuln-finder

#### 目的

极大程度且精确的获取互联网上的漏洞情报

#### 设想

强大的信息收集模块和多种数据挖掘模块的框架，输出精确简练的结果便于学习和研究只用。目前只专注于漏洞情报的收集，设计时考虑未来可自定义信息收集的种类。

#### v1.0bate需求

- 收集模块
  
  > 输出爬取的最新资讯，具有扩展性以插件的形式针对某一特定平台添加特定的插件。（未来可通过自学习生成插件）
  
  - [x] 知名媒体发布
  - [x] 安全厂商预警
  - [ ] 漏洞平台更新
  - [ ] 个人博客
  - [ ] 众测平台报告
  - [ ] 各大公众号
  - [ ] 。。。
  
- 分析模块

  - [x] 识别确认
  - [ ] 分类（可利用程度、有无POC/EXP）
  - [ ] 权重覆盖（针对确定的漏洞深入搜索，权重更新覆盖掉权重较低的信息）
  - [ ] 相关性搜索（搜索POC、EXP）
  - [ ] 提炼核心
  - [ ] 。。。

- 输出模块

  - [x] 文本txt
  - [ ] 页面html
  - [ ] webhook(json)对接各类机器人
  - [ ] 时间线（针对同一漏洞建立时间线）
  - [ ] 。。。

#### 技术栈

##### 开发语言

##### Python

- 优点
  - 有现成的爬虫框架
- 缺点
  - 对不规范HTML适应能力差。如处理不同编码集的数据。

##### GO

- 优点
  - 线程调度简单，支持高并发。
- 缺点
  - 需要编译

#### 爬虫先用Python写, 数据分析及其他功能待定
##### 开发环境
- python版本3.7
- 命名规范
  - 驼峰命名 
  - 成员变量 m_bxxx
  - 局部变量命名前缀加变量类型， 如： bFlag
  - 私有函数，前缀加下划线_
  - 全局常量，全部大写，中间加下划线， 如：MY_NAME
  - 全局变量: g_XXX

##### 开源成熟框架参考

##### 参考资料
 -https://www.zhihu.com/question/60280580/answer/617068010 
