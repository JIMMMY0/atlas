# System Engineering of SpaceX

笔者按：我们曾经从教科书上、从专家的讲座里获得的“系统工程”种种教诲，有很大部分可能已经失效了。那些东西是从上个世纪五、六十年代阿波罗登月计划开始发展起来的，这套方法论创造了我们现在看到的波音、空客、登月、航母等巨型工程。然而，用埃隆马斯克的话说：“现在是21世纪！”

文末有重大福利：《SpaceX内部讲义之系统工程》

在最近SpaceX Falcon Heavy（猎鹰重型）成功发射后，我一直苦苦思考：**一个成立初只有几十个人，到2008年才500人，一直到现在有4000多人的民营公司，如何支撑起如此庞大的系统工程？**要知道，无论是美国，还是中国，都有数十万计的人在庞大的、由政府直接干预的机构里从事着这样的事业。

查阅了一些文献，我惊讶的发现：我们曾经从教科书上、从专家的讲座里获得的“系统工程”种种教诲，有很大部分可能已经失效，或者需要我们重新审视。那些东西是从上个世纪五、六十年代阿波罗登月计划开始发展起来的，这套方法论创造了我们现在看到的波音、空客、登月、航母等巨型工程。然而，用埃隆马斯克的话说：“现在是21世纪！”

**一、时代变了**

如果让你从头开始研制波音747，你会翻开一本讲述系统工程的经典教材，它会向你讲述波音公司1960年如何启动这个项目，以及1969年如何成功交付的。你会惊叹在那样一个年代，9年即可交付，这简直就是一个奇迹。在这种情绪的带动下，你也许会照搬了书上说的那套波音公司的方法论。

**然而，时代变了。现在距离1960年将近60年过去了！**

SpaceX对系统工程的描述中，有一句提纲挈领的话值得深思：“A Traditional Discipline in a Non-traditional Organization”（新组织中的旧学科）。

马斯克一直对团队强调一个词，叫“21th Century Infrastructure”（21世纪基础设施）。有哪些？我们可以罗列一下：

新的沟通效率、新的资源获取效率、新的协作关系、新工具、新工艺、新技术，等等。

由于复杂系统是永恒存在的，所以这些新的东西不会否定“系统工程”这门学科的存在。所以，SpaceX颠覆的不是系统工程，而是传统系统工程中的诸多理念。

**二、过度的“前期设计”**

传统的系统工程告诉我们，在前期设计中暴露尽可能多的风险，以降低错误成本。这种教诲让我们现在很多大型项目在前期设计上大量地耗费时间和精力，以至于迟迟不去实践**。我们越来越信奉“一次成功”这样的口号，这听起来很节约成本，然而在时间和人力可以与资本兑换的时代，在试错成本上，我们是否应该寻找新的平衡点？**

![](data:image/gif;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVQImWNgYGBgAAAABQABh6FO1AAAAABJRU5ErkJggg==)

↑考虑资金成本的传统模型

![](data:image/gif;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVQImWNgYGBgAAAABQABh6FO1AAAAABJRU5ErkJggg==)

↑SpaceX考虑综合成本的新模型

SpaceX更强调每一次完整迭代之后产生的“经验”，他们认为，基于更先进的工具和更优化的供应链协作关系，这种走完多次“设计、开发、测试”流程所需要的成本已经大大低于上个世纪；而每一次完整迭代之后产生的经验，实际上是降低了项目的整体成本。

**三、由需求层次驱动的迭代设计**

“迭代设计”是我们经常提到的，在迭代设计中，我们强调快速将产品原型呈现给用户，然后再做迭代，这种迭代的目的是为了优化产品的需求。为了能够使用户提出更多的建议，我们在每一次迭代中往往倾向于尽可能挖掘原型的需求纵深，以尽可能减少迭代次数。

而SpaceX认为：迭代的核心目的是为了获取经验，根据人类认知的规律，需求纵深的挖掘应该在迭代的过程中进行，也就是“由需求层次驱动迭代”。

笔者的理解是：刚开始更关注上层关键需求，对于下层的需求，可以先不关注，先采用既有的或者是成本较低的方案实现，等上层的关键需求都实现之后，再将下层需求的实现进行逐步迭代。我们看下面两张图就能明白了：

![](data:image/gif;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVQImWNgYGBgAAAABQABh6FO1AAAAABJRU5ErkJggg==)

传统的V模型

（笔者注：传统V模型的左侧，在前期就将需求从Level 2推演到Level 4，这就是我们通常说的“需求分析”）

![](https://mmbiz.qpic.cn/mmbiz_png/At56A9SyicgKoeoCPfYZ3w9Ub1uyZF6ib41YCLiaW5hgWQ4Xs5aIQGUghiaXPIYzrWa8nhqho4tWGGZmUrnvYM8ibLw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)

SpaceX的V模型——第一轮迭代

我们发现，SpaceX的V模型中，第一轮迭代时没有出现Level 3和Level 4层次的需求，但是十分强调Key Design Parameters（关键设计参数），也就是说，对于那些lower level requirements（即Level 3和Level 4的需求），等关键需求被满足和验证之后，再逐步迭代实现。

设计实例：

> 以发动机控制为例，在Level 2 Requirements阶段是这样的：
>
> ![](https://mmbiz.qpic.cn/mmbiz_png/At56A9SyicgKoeoCPfYZ3w9Ub1uyZF6ib4OuYS6tXwb2RVeh0zdJ2C747o4zialqhnS2KxWTPBCLGd6IibgdYFYFAw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)
>
> 但是到了Lower Level Requirements阶段时，变成了这样：
>
> ![](https://mmbiz.qpic.cn/mmbiz_png/At56A9SyicgKoeoCPfYZ3w9Ub1uyZF6ib4WqtZZHO3X23j4WmUkJoCEIBtmsaNdoB8bJib5zNzV5HiafuBZic17zZug/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)

**四、实现低层次需求的能力**

这是一个十分关键的概念，我想重点说一下。

SpaceX的原文描述是：ability to trade lower level requirements，所以有技术类文章把它翻译成“交易低层次需求的能力”，并诠释为：与用户交易，劝说用户那些不重要的需求就放弃吧；与转包者交易，希望对方既快且经济地交出产品。虽然这话说得没错，但这是基于错误理解的翻译，我查阅了SpaceX很多文章，没有发现SpaceX具有将这种lower level requirements向用户进行交易的能力和行为。

笔者的理解是：**一般总体单位只关注顶层需求（Level 2），对于低层次的Level 3和Level 4需求往往通过外协的方式进行分包；而SpaceX则不认同这一观点，要知道，一支火箭70%干重（硬件）的设备都是由SpaceX自己设计的。**

我们从下面的两张图中可以发现：

![](https://mmbiz.qpic.cn/mmbiz_png/At56A9SyicgKicUjFlD0zQZlOw6tSQrqiasJKlqZvcrclW8QUfGOvbI5WrXsvNODSRXnwL3UAoYN9679EhFlfjb3g/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)

↑传统的总体单位分包模式（图中A是Tier-1总体单位，其他字母表示Tier-2和Tier-3的供应商）

![](https://mmbiz.qpic.cn/mmbiz_png/At56A9SyicgKicUjFlD0zQZlOw6tSQrqiasMH5AaLbePStU25LqlsnoNptpDo2DMK12iaFezpLjW1EbKwRWMOtgAkg/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)

↑SpaceX的总体分包模式

显而易见的是，SpaceX把我们认为该给供应商的干的大部分活儿，自己都干完了。当然，他只是自己设计。

**五、“创新力”与“规范、过程”之间的矛盾**

在一个庞大的系统工程中，管理者试图通过严格的规范和过程管理来实现对项目的控制。很多项目团队甚至大量引进制造型企业的一套过程管理方法。

SpaceX一直在寻求一种平衡，为了使团队保有创新能力，他们一直尝试着精简组织架构、省略更多的规范、去除不必要的过程管理，**SpaceX将系统工程的管理建立在每个员工的“责任心”基础之上，这是SpaceX的核心理念，“想正确、高效地完成任务，任何现有的过程管理都无法取代责任心”**。

这给管理提出一个新的要求，**过去，我们从流水线上总结出“用制度替代人性“的管理要义；今天，在需要发挥每个人创新力的时代，我们是否应该反其道而行之，”用人性替代制度“？**

实际上，上文提到的每一个点，都是值得深入研究的，我们不确定SpaceX是如何具体实践这些理念的，但我们应该思考新的理念并且大胆实践。

{% file src="../.gitbook/assets/case2012\_2-4\_muratore\_presentation.pdf" caption="System Engineering: A Traditional Discipline to a Non-traditional Organization" %}

{% api-method method="get" host="" path="" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

