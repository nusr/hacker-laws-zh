# 💻📖 黑客定律

[![Build Status](https://travis-ci.org/nusr/hacker-laws-zh.svg?branch=master)](https://travis-ci.org/nusr/hacker-laws-zh)

[hacker-laws](https://github.com/dwmkerr/hacker-laws) 的的中文翻译。

对开发人员有用的定律，理论，原则和模式。(Laws, Theories, Principles and Patterns that developers will find useful.)

为了方便阅读，维基百科增加了中文链接！

英文链接表示 [hacker-laws](https://github.com/dwmkerr/hacker-laws) 项目尚未完成的主题。

[中国无法访问维基百科说明](gfw.md)

喜欢点 **star** 、关注点 **watch**、贡献点 **fork** 。

- [介绍](#%E4%BB%8B%E7%BB%8D)
- [定律](#%E5%AE%9A%E5%BE%8B)
  - [阿姆达尔定律 (Amdahl's Law)](#%E9%98%BF%E5%A7%86%E8%BE%BE%E5%B0%94%E5%AE%9A%E5%BE%8B-amdahls-law)
  - [布鲁克斯法则 (Brooks's Law)](#%E5%B8%83%E9%B2%81%E5%85%8B%E6%96%AF%E6%B3%95%E5%88%99-brookss-law)
  - [康威定律 (Conway's Law)](#%E5%BA%B7%E5%A8%81%E5%AE%9A%E5%BE%8B-conways-law)
  - [侯世达定律 (Hofstadter's Law)](#%E4%BE%AF%E4%B8%96%E8%BE%BE%E5%AE%9A%E5%BE%8B-hofstadters-law)
  - [技术成熟度曲线 (The Hype Cycle & Amara's Law)](#%E6%8A%80%E6%9C%AF%E6%88%90%E7%86%9F%E5%BA%A6%E6%9B%B2%E7%BA%BF-the-hype-cycle--amaras-law)
  - [隐式接口定律 (Hyrum's Law)](#%E9%9A%90%E5%BC%8F%E6%8E%A5%E5%8F%A3%E5%AE%9A%E5%BE%8B-hyrums-law)
  - [摩尔定律 (Moore's Law)](#%E6%91%A9%E5%B0%94%E5%AE%9A%E5%BE%8B-moores-law)
  - [帕金森定理 (Parkinson's Law)](#%E5%B8%95%E9%87%91%E6%A3%AE%E5%AE%9A%E7%90%86-parkinsons-law)
  - [普特定律 (Putt's Law)](#%E6%99%AE%E7%89%B9%E5%AE%9A%E5%BE%8B-putts-law)
  - [复杂性守恒定律 (The Law of Conservation of Complexity)](#%E5%A4%8D%E6%9D%82%E6%80%A7%E5%AE%88%E6%81%92%E5%AE%9A%E5%BE%8B-the-law-of-conservation-of-complexity)
  - [漏洞抽象定律 (The Law of Leaky Abstractions)](#%E6%BC%8F%E6%B4%9E%E6%8A%BD%E8%B1%A1%E5%AE%9A%E5%BE%8B-the-law-of-leaky-abstractions)
  - [帕金森琐碎定理 (The Law of Triviality)](#%E5%B8%95%E9%87%91%E6%A3%AE%E7%90%90%E7%A2%8E%E5%AE%9A%E7%90%86-the-law-of-triviality)
  - [Unix 哲学 (The Unix Philosophy)](#unix-%E5%93%B2%E5%AD%A6-the-unix-philosophy)
  - [Spotify 模型 (The Spotify Model)](#spotify-%E6%A8%A1%E5%9E%8B-the-spotify-model)
  - [沃德勒定律 (Wadler's Law)](#%E6%B2%83%E5%BE%B7%E5%8B%92%E5%AE%9A%E5%BE%8B-wadlers-law)
- [原则](#%E5%8E%9F%E5%88%99)
  - [鲁棒性原则 (The Robustness Principle)](#%E9%B2%81%E6%A3%92%E6%80%A7%E5%8E%9F%E5%88%99-the-robustness-principle)
  - [SOLID](#solid)
  - [单一功能原则 (The Single Responsibility Principle)](#%E5%8D%95%E4%B8%80%E5%8A%9F%E8%83%BD%E5%8E%9F%E5%88%99-the-single-responsibility-principle)
  - [开闭原则 (The Open/Closed Principle)](#%E5%BC%80%E9%97%AD%E5%8E%9F%E5%88%99-the-openclosed-principle)
  - [里氏替换原则 (The Liskov Substitution Principle)](#%E9%87%8C%E6%B0%8F%E6%9B%BF%E6%8D%A2%E5%8E%9F%E5%88%99-the-liskov-substitution-principle)
  - [接口隔离原则 (The Interface Segregation Principle)](#%E6%8E%A5%E5%8F%A3%E9%9A%94%E7%A6%BB%E5%8E%9F%E5%88%99-the-interface-segregation-principle)
  - [依赖反转原则 (The Dependency Inversion Principle)](#%E4%BE%9D%E8%B5%96%E5%8F%8D%E8%BD%AC%E5%8E%9F%E5%88%99-the-dependency-inversion-principle)
- [TODO](#todo)

## 介绍

当人们谈论开发时，会聊到许多定律。 这个仓库收录了一些最常见的定律。请分享这个仓库并提交 PR ！

❗: 这个仓库包含对一些定律、原则以及模式的解释，但不**提倡**其中任何一个。 它们的应用始终存在着争论，并且很大程度上取决于你正在做什么。

## 定律

现在我们开始吧！

### 阿姆达尔定律 (Amdahl's Law)

- [英文维基百科](https://en.wikipedia.org/wiki/Amdahl%27s_law)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E9%98%BF%E5%A7%86%E8%BE%BE%E5%B0%94%E5%AE%9A%E5%BE%8B)

> 阿姆达尔定律是一个显示计算任务**潜在加速**能力的公式。这种能力可以通过增加系统资源来实现，通常用于并行计算中。它可以预测增加处理器数量的实际好处，然而增加处理器数量会受到程序并行性的限制。

举例说明：如果程序由两部分组成，部分 A 必须由单个处理器执行，部分 B 可以并行运行。那么向执行程序的系统添加多个处理器只能获得有限的好处。它可以极大地提升部分 B 的运行速度，但部分 A 的运行速度将保持不变。

下图展示了运行速度的潜能：

![阿姆达尔定律](./images/amdahls_law.png)

_(图片来源: By Daniels220 at English Wikipedia, Creative Commons Attribution-Share Alike 3.0 Unported, https://en.wikipedia.org/wiki/File:AmdahlsLaw.svg)_

可以看出，50％ 并行化的程序仅仅受益于 10 个处理单元，而 95％ 并行化的程序可以通过超过一千个处理单元显著提升速度。

随着摩尔定律减慢，以及单个处理器的速度增加缓慢，并行化是提高性能的关键。图形编程是一个极好的例子，现代着色器可以并行渲染单个像素或片段。这也是为什么现代显卡通常具有数千个处理核心（GPU 或着色器单元）的原因。

参见：

- [布鲁克斯法则](#%E5%B8%83%E9%B2%81%E5%85%8B%E6%96%AF%E6%B3%95%E5%88%99-brookss-law)
- [摩尔定律](#%E6%91%A9%E5%B0%94%E5%AE%9A%E5%BE%8B-moores-law)

### 布鲁克斯法则 (Brooks's Law)

- [英文维基百科](https://en.m.wikipedia.org/wiki/Brooks%27s_law)

布鲁克斯是《人月神话》的作者。

> 软件开发后期，添加人力只会使项目开发得更慢。

这个定律表明，在许多情况下，试图通过增加人力来加速延期项目的交付，将会使项目交付得更晚。布鲁克斯也明白，这是一种过度简化。但一般的推理是，新资源的增加时间和通信开销，会使开发速度减慢。而且，许多任务是不可分的，比如更多的资源容易分配，这也意味着潜在的速度增加也更低。

谚语 **九个女人不能在一个月内生一个孩子** 与布鲁克斯法则同出一辙，特别是某些不可分割或者并行的工作。

参见：

- [Death March](#todo)

### 康威定律 (Conway's Law)

- [英文维基百科](https://en.wikipedia.org/wiki/Conway%27s_law)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E5%BA%B7%E5%A8%81%E5%AE%9A%E5%BE%8B)

系统的技术边界受制于组织的结构。改进组织时，通常会提到它。康威定律表明，如果一个组织被分散成许多小而无联系的单元，那么它开发的软件也是小而分散的。如果一个组织更多地垂直建立在特性或其服务周围，那么软件系统也会反映这一点。

参见：

- [The Spotify Model](#spotify-%E6%A8%A1%E5%9E%8B-the-spotify-model)

### 侯世达定律 (Hofstadter's Law)

- [英文维基百科](https://en.wikipedia.org/wiki/Hofstadter%27s_law)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E4%BE%AF%E4%B8%96%E8%BE%BE%E5%AE%9A%E5%BE%8B)

> 即使考虑到侯世达定律，它也总是比你预期的要长。

在估计需要多长时间开发时，你可能会听到此定律。软件开发似乎不言而喻，我们往往不能准确地估计需要多长时间才能完成。

### 技术成熟度曲线 (The Hype Cycle & Amara's Law)

- [英文维基百科](https://en.wikipedia.org/wiki/Hype_cycle)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E6%8A%80%E6%9C%AF%E6%88%90%E7%86%9F%E5%BA%A6%E6%9B%B2%E7%BA%BF)

> 我们倾向于过高估计技术在短期内的影响，并低估长期效应。
>
> (罗伊·阿马拉)

技术成熟度曲线是[高德纳咨询公司](https://zh.wikipedia.org/wiki/%E9%AB%98%E5%BE%B7%E7%BA%B3%E5%92%A8%E8%AF%A2%E5%85%AC%E5%8F%B8)对技术最初兴起和发展的视觉展现。一图顶千言：

![The Hype Cycle](./images/gartner_hype_cycle.png)

_(图片来源: By Jeremykemp at English Wikipedia, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=10547051)_

简而言之，这个周期表明，新技术及其潜在影响通常会引发一阵浪潮。团队快速使用这些新技术，有时会对结果感到失望。这可能是因为该技术还不够成熟，或者现实应用还没有完全实现。经过一段时间后，技术的能力提高了，使用它的实际机会会增加，最终团队也可以提高工作效率。罗伊·阿马拉简洁地总结了这一点：我们倾向于高估技术短期内的影响，并低估长期效应。

### 隐式接口定律 (Hyrum's Law)

- [英文在线地址](http://www.hyrumslaw.com/)

> API 有足够多的用户。
> 你在合同中的承诺并不重要：
> 你系统的所有可观察行为将取决于其他人。
>
> （Hyrum Wright）

隐式接口定律表明，当你的 API 有足够多的用户时，API 的所有行为（即使那些未被定义为公共说明的一部分）最终都会被其他人所依赖。 一个简单的例子，例如 API 的响应时间这种非功能性因素。 一个更微妙的例子是：用户使用正则表达式判断错误信息的类型时，即使 API 的公共说明没有说明消息的内容，来指示用户错误的类型。一些用户可能会使用该消息，并且更改该消息。实际上会破坏 API 的使用。

参见：

- [漏洞抽象定律](#%E6%BC%8F%E6%B4%9E%E6%8A%BD%E8%B1%A1%E5%AE%9A%E5%BE%8B-the-law-of-leaky-abstractions)

### 摩尔定律 (Moore's Law)

- [英文维基百科](https://en.wikipedia.org/wiki/Moore%27s_law)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E6%91%A9%E5%B0%94%E5%AE%9A%E5%BE%8B)

> 集成电路中的晶体管数量大约每两年翻一番。

通常用于说明半导体和芯片技术提高的绝对速度。从 20 世纪 70 年代到 21 世纪后期，摩尔的预测被证明是高度准确的。 近年来，这种趋势略有变化，部分原因受到[量子隧穿效应](https://zh.wikipedia.org/wiki/%E9%87%8F%E5%AD%90%E7%A9%BF%E9%9A%A7%E6%95%88%E6%87%89)影响。然而，并行化计算的进步以及半导体技术和量子计算潜在的革命性变化，可能意味着摩尔定律在未来几十年内继续保持正确。

### 帕金森定理 (Parkinson's Law)

- [英文维基百科](https://en.wikipedia.org/wiki/Parkinson%27s_law)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E5%B8%95%E9%87%91%E6%A3%AE%E5%AE%9A%E7%90%86)

> 在工作能够完成的时限内，工作量会一直增加，直到所有可用时间都被填满为止。

基于官僚机构的研究背景，该定律被应用于软件开发中。该理论认为，团队在截止日期之前效率低下，然后在截止日期前赶紧完成工作，从而使实际截止日期变得随意。

将这个定理与[侯世达定律](#%E4%BE%AF%E4%B8%96%E8%BE%BE%E5%AE%9A%E5%BE%8B-hofstadters-law)相结合，则会获得更加悲观的观点：为了在规定时间内完成工作，工作将增多，花费比预期更长的时间。

参见：

- [侯世达定律](#%E4%BE%AF%E4%B8%96%E8%BE%BE%E5%AE%9A%E5%BE%8B-hofstadters-law)

### 普特定律 (Putt's Law)

- [英文维基百科](https://en.wikipedia.org/wiki/Putt%27s_Law_and_the_Successful_Technocrat)

> 技术由两类人主导，一类是纯粹的管理人员， 一类是纯粹的技术人员。

普特定律常常遵循普特推论：

> 每一个技术层次，假以时日，能力将逆转。

这些结论表明，由于各种选择标准和群体组织的趋势，技术组织的工作层面将有一些技术人员，以及一些不了解复杂性和挑战的管理人员。这种现象可能是由于 [The Peter Principe](#TODO) 或 [Dilbert's Law](#TODO) 造成的。

但是，应该强调的是，诸如此类的定律是一种广泛的概括，可能适用于某些类型的组织，而不适用于其他组织。

参见：

- [The Peter Principe](#TODO)
- [Dilbert's Law](#TODO).

### 复杂性守恒定律 (The Law of Conservation of Complexity)

- [英文维基百科](https://en.wikipedia.org/wiki/Law_of_conservation_of_complexity)

该定律表明系统中存在着一定程度的复杂性，并且不能减少。

系统中的某些复杂性是**无意的**。这是由于结构不良，错误或者糟糕的建模造成的。可以减少以及消除无意的复杂性。然而，由于待解决问题固有的复杂性，某些复杂性是**内在的**。这种复杂性可以转移，但不能消除。

该定律有趣的一点是，即使简化整个系统，内在的复杂性也不会降低。它会**转移到用户**，并且用户必须以更复杂的方式行事。

### 漏洞抽象定律 (The Law of Leaky Abstractions)

- [英文在线地址](https://www.joelonsoftware.com/2002/11/11/the-law-of-leaky-abstractions/)

> 在某种程度上，所有非平凡的抽象都是漏洞。
>
> (乔尔斯·波尔斯基)

该定律指出，通常用于简化复杂系统的抽象，某些情况下将在底层系统爆出漏洞，这使得抽象表现为意外的方式。

例如加载文件并读取其内容。文件系统 API 是较低级别内核系统的抽象，它们本身是与磁盘（或 SSD 的闪存）上的数据更改相关的物理过程抽象。在大多数情况下，处理文件（如二进制数据流）的抽象将起作用。但是，对于磁盘驱动器，顺序读取数据将比随机访问快得多（由于页面错误的开销增加）。但对于 SSD 驱动器，此开销不会出现。需要理解基础细节来处理这种情况（例如，数据库索引文件的良好结构可以减少随机访问的开销），开发人员需要合理的抽象，来处理不同的细节。

当引入的抽象更多时，上面的例子会变得更复杂。Linux 操作系统允许通过网络访问文件，但在本地表示为普通文件。如果存在网络故障，这种抽象将有漏洞。如果开发人员将这些文件视为普通文件，而不考虑它们可能会受到网络延迟和故障的影响，那么解决方案就会出错。

描述该定律的文章表明，过度依赖抽象，加上对底层过程的理解不足，实际上使得问题在某些情况下更加复杂。

参见：

- [隐式接口定律](#%E9%9A%90%E5%BC%8F%E6%8E%A5%E5%8F%A3%E5%AE%9A%E5%BE%8B-hyrums-law)

真实的例子：

- [Photoshop 启动缓慢](https://forums.adobe.com/thread/376152)：我过去遇到过一个问题，就是 Photoshop 启动缓慢，有时需要几分钟。问题好像是 Photoshop 启动时，会读取当前默认打印机的一些信息。但是，如果该打印机实际上是一台网络打印机，则可能需要很长的时间。将网络打印机与本地打印机当作同样的抽象，导致连接不良的情况下出现问题。

### 帕金森琐碎定理 (The Law of Triviality)

- [英文维基百科](https://en.wikipedia.org/wiki/Law_of_triviality)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E5%B8%95%E9%87%91%E6%A3%AE%E7%91%A3%E7%A2%8E%E5%AE%9A%E7%90%86)

该定理显示，群体将给予更多的时间和注意力来处理琐碎的问题，而不是用来处理严肃而实质性的问题。

常见的虚构例子是委员会批准核电站的计划，他们大部分时间都在讨论自行车棚的结构，而不是电厂本身等更为重要的设计。如果没有大量的专业知识或者准备，很难给非常大的复杂主题讨论提供宝贵的意见。但是，人们希望看到更多意见。因此，倾向于将过多的时间集中在小细节上，这很容易推理，但不被看重。

上面的虚构例子导致使用**Bike Shedding**这个词，作为在琐碎细节上浪费时间的表达。

### Unix 哲学 (The Unix Philosophy)

- [英文维基百科](https://en.wikipedia.org/wiki/Unix_philosophy)
- [中文维基百科](https://zh.wikipedia.org/wiki/Unix%E5%93%B2%E5%AD%A6)

Unix 哲学指软件组件应该很小，并专注于做一件特定的事情。将小而简单以及定义良好的单元组合在一起，而不是使用大而复杂的多用途程序，可以更轻松地构建系统。

像**微服务架构**这种现代实践可以认为是这种哲学的应用，其中服务很小，集中于做一件特定的事情，由简单的构建块组成复杂的行为。

### Spotify 模型 (The Spotify Model)

- [英文在线地址](https://labs.spotify.com/2014/03/27/spotify-engineering-culture-part-1/)

Spotify 模型是团队和组织结构的一种方法，已被 Spotify 实验室推广开来。在此模型中，团队围绕功能而非技术进行组织。

Spotify 模型还普及了部落、行会以及章节的概念，这些是其组织结构的其他组成部分。

### 沃德勒定律 (Wadler's Law)

- [英文在线地址](https://wiki.haskell.org/Wadler's_Law)

> 任何语言设计中，讨论下面列表中某个要素所花费的总时间与其位置成正比。
>
> 0. 语义 (Semantics)
> 1. 语法 (Syntax)
> 2. 词法 (Lexical syntax)
> 3. 注释语法 (Lexical syntax of comments)
>
> （简而言之，在语义上花费一个小时，就要在注释语法上花费八个小时）。

与 [帕金森琐碎定理](#%E5%B8%95%E9%87%91%E6%A3%AE%E7%90%90%E7%A2%8E%E5%AE%9A%E7%90%86-the-law-of-triviality) 类似, 沃德勒定律指出，在设计语言时，与这些特征的重要性相比，花在语言结构上的时间过多。

参见：

- [帕金森琐碎定理](#%E5%B8%95%E9%87%91%E6%A3%AE%E7%90%90%E7%A2%8E%E5%AE%9A%E7%90%86-the-law-of-triviality)

## 原则

原则通常是与设计相关的准则。

### 鲁棒性原则 (The Robustness Principle)

- [英文维基百科](https://en.wikipedia.org/wiki/Robustness_principle)

> 在自己所做的事情上要保守, 在接受别人的事情上要自由。

通常应用于服务器应用程序开发中，该原则指出，你发送给其他人的内容应尽可能最小且符合要求，并且处理不符合要求的输入。

该原则的目标是构建稳健的系统。如果可以理解意图，它们可以处理不良的输入。但是，接受错误格式的输入可能存在安全隐患，特别是此类的输入未经过充分测试。

### SOLID

这是一个缩写，指的是：

- S：[单一功能原则 (The Single Responsibility Principle)](#%E5%8D%95%E4%B8%80%E5%8A%9F%E8%83%BD%E5%8E%9F%E5%88%99-the-single-responsibility-principle)
- O：[开闭原则 (The Open/Closed Principle)](#%E5%BC%80%E9%97%AD%E5%8E%9F%E5%88%99-the-openclosed-principle)
- L：[里氏替换原则 (The Liskov Substitution Principle)](#%E9%87%8C%E6%B0%8F%E6%9B%BF%E6%8D%A2%E5%8E%9F%E5%88%99-the-liskov-substitution-principle)
- I：[接口隔离原则 (The Interface Segregation Principle)](#%E6%8E%A5%E5%8F%A3%E9%9A%94%E7%A6%BB%E5%8E%9F%E5%88%99-the-interface-segregation-principle)
- D：[依赖反转原则 (The Dependency Inversion Principle)](#%E4%BE%9D%E8%B5%96%E5%8F%8D%E8%BD%AC%E5%8E%9F%E5%88%99-the-dependency-inversion-principle)

这些是 [Object-Oriented Programming](#todo) 的关键原则。诸如此类的设计原则能够帮助开发人员构建更易于维护的系统。

### 单一功能原则 (The Single Responsibility Principle)

- [英文维基百科](https://en.wikipedia.org/wiki/Single_responsibility_principle)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E5%8D%95%E4%B8%80%E5%8A%9F%E8%83%BD%E5%8E%9F%E5%88%99)

> 每个模块或者类只应该有一项功能。

[SOLID](#solid) 的第一个原则。这个原则表明模块或者类只应该做一件事。实际上，这意味着对程序功能的单个小更改，应该只需要更改一个组件。例如，更改密码验证复杂性的方式应该只需要更改程序的一部分。

理论上讲，这使代码更健壮，更容易更改。知道正在更改的组件只有一个功能，这意味着测试更改更容易。使用前面的例子，更改密码复杂性组件应该只影响与密码复杂性相关的功能。变更具有许多功能的组件可能要困难得多。

参见：

- [Object-Orientated Programming](#todo)
- [SOLID](#solid)

### 开闭原则 (The Open/Closed Principle)

- [英文维基百科](https://en.wikipedia.org/wiki/Open%E2%80%93closed_principle)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E5%BC%80%E9%97%AD%E5%8E%9F%E5%88%99)

> 实体应开放扩展并关闭修改。

[SOLID](#solid) 的第二个原则。这个原则指出实体（可以是类、模块、函数等）应该能够使它们的行为易于扩展，但是它们的扩展行为不应该被修改。

举一个假设的例子，想象一个能够将 Markdown 转换为 HTML 的模块。如果可以扩展模块，而不修改内部模块来处理新的 markdown 特征，而无需修改内部模块，则可以认为是开放扩展。如果用户不能修改模块以处理现有的 Markdown 特征，那么它被认为是关闭修改。

这个原则与面向对象编程紧密相关，让我们可以设计对象以便于扩展，但是可以避免以意想不到的方式改变其现有对象的行为。

参见：

- [Object-Orientated Programming](#todo)
- [SOLID](#solid)

### 里氏替换原则 (The Liskov Substitution Principle)

- [英文维基百科](https://en.wikipedia.org/wiki/Liskov_substitution_principle)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E9%87%8C%E6%B0%8F%E6%9B%BF%E6%8D%A2%E5%8E%9F%E5%88%99)

> 可以在不破坏系统的情况下，用子类型替换类型。

[SOLID](#solid) 的第三个原则。该原则指出，如果组件依赖于类型，那么它应该能够使用该类型的子类型，而不会导致系统失败或者必须知道该子类型的详细信息。

举个例子，假设我们有一个方法，读取 XML 文档。如果该方法使用基类型 **file**，则从 **file** 派生的任何内容，都能用在该方法中。 如果 **file** 支持反向查找，并且 xml 解析器使用该函数，但是派生类型 **network file** 尝试反向查找时失败，则 **network file** 将违反该原则。

该原则与面向对象编程特别有关，必须仔细建模类型、层次结构，以避免混淆系统用户。

参见：

- [Object-Orientated Programming](#todo)
- [SOLID](#solid)

### 接口隔离原则 (The Interface Segregation Principle)

- [英文维基百科](https://en.wikipedia.org/wiki/Interface_segregation_principle)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E6%8E%A5%E5%8F%A3%E9%9A%94%E7%A6%BB%E5%8E%9F%E5%88%99)

> 不应强制任何客户端依赖于它不使用的方法。

[SOLID](#solid) 的第四个原则。该原则指出组件的消费者不应该依赖于它实际上不使用的组件函数。

举一个例子，假设我们有一个方法，读取 XML 文档。它只需要读取文件中的字节，向前移动或向后移动。如果由于文件结构不相关（例如更新文件安全性的权限模型），需要更新此方法，则该原则已失效。文件最好实现 **可查询流** 接口，并让 XML 读取器使用该接口。

该原则与面向对象编程紧密相关，其中接口，层次结构和抽象类型用于不同组件的 [minimise the coupling](#todo)。 [Duck typing](#todo) 是一种通过消除显式接口来强制执行该原则的方法。

参见：

- [Object-Orientated Programming](#todo)
- [SOLID](#solid)
- [Duck Typing](#todo)
- [Decoupling](#todo)

### 依赖反转原则 (The Dependency Inversion Principle)

- [英文维基百科](https://en.wikipedia.org/wiki/Dependency_inversion_principle)
- [中文维基百科](https://zh.wikipedia.org/wiki/%E4%BE%9D%E8%B5%96%E5%8F%8D%E8%BD%AC%E5%8E%9F%E5%88%99)

> 高级模块不应该依赖于低级实现。

[SOLID](#solid) 的第五个原则。该原则指出，更高级别的协调组件不应该知道其依赖项的详细信息。

举个例子，假设我们有一个从网站读取元数据的程序。我们假设主要组件必须知道下载网页内容的组件，以及可以读取元数据的组件。如果我们考虑依赖反转，主要组件将仅依赖于可以获取字节数据的抽象组件，然后是一个能够从字节流中读取元数据的抽象组件。主要组件不需要了解 TCP、IP、HTTP、HTML 等。

这个原则很复杂，因为它似乎可以反转系统的预期依赖性（因此得名）。实践中，这也意味着，单独的编排组件必须确保抽象类型的正确实现被使用（例如在前面的例子中，必须提供元数据读取器组件、HTTP 文件下载功能和 HTML 元标签读取器）。然后，这涉及诸如 [Inversion of Control](#todo) 和 [Dependency Injection](#todo) 之类的模式。

参见：

- [Object-Orientated Programming](#todo)
- [SOLID](#solid)
- [Inversion of Control](#todo)
- [Dependency Injection](#todo)

## TODO

嗨！如果你读到这里，点击了一个我尚未编写的主题链接，我感到抱歉。 这是正在进行中的工作！

随意提 [Issue](https://github.com/dwmkerr/hacker-laws/issues) 获取更多详细信息，或者 [Pull Request](https://github.com/dwmkerr/hacker-laws/pulls) 提交你提议的主题。
