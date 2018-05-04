> 根据自己理解进行一次可读化的翻译。

## Steem
基于区块链的激励式公共内容平台。
> An incentivized, blockchain-based, public content platform.
August 2017

## 摘要 - Abstract
Steem是一个支持社区建设与加密货币奖励社交互动的区块链。Steem将社交媒体、加密货币及社区建设相结合。鼓励参与任何社区、货币或自由市场经济的一个重要关键是：公正的会计制度，它将始终反映着每个人的贡献。Steem是第一个试图准确和透明的奖励无数为社区做出主观贡献者的加密货币。

> Steem is a blockchain database that supports community building and social interaction
with cryptocurrency rewards. Steem combines concepts from social media with lessons
learned from building cryptocurrencies and their communities. An important key to
inspiring participation in any community, currency or free market economy is a fair
accounting system that consistently reflects each person's contribution. Steem is the first
cryptocurrency that attempts to accurately and transparently reward an unbounded
number of individuals who make subjective contributions to its community.

## 目录 - Table of Contents
- 摘要（Abstract）
- 目录（Table of Contents）
- 简介（Introduction）
    - 识别贡献（Recognizing Contribution）
- 贡献方式（Ways to Contribute）
    - 资本投入（Capital Contributions）
    - Steem （STEEM）
    - Steem Power（SP）
    - Steem Dollars（SBD）
        - 最小化欺骗行为（Minimizing Fraudulent Feeds）
        - 弱化时间差攻击（Mitigating Timing Attacks）
        - 最小化价值转换（Minimizing Abuse of Conversions）
        - 可持续债务与所有权比率（Sustainable Debt to Ownership Ratios）
        - 利息（Interest）
        - 价格调控机制（Setting Price Feeds）
    - 主观的贡献（Subjective Contributions）
        - 货币分配（Distributing Currency）
        - 货币分配投票机制（Voting on Distribution of Currency）
             - 投票舞弊（Voting Abuse）
             - 螃蟹桶的故事（The Story of the Crab Bucket）
        - 投票速度的限制（Rate Limited Voting）
        - 奖励分配（Payout Distribution）
        - 支出（Payouts）
- 共识算法（Consensus Algorithm）
    - Steem共识（Consensus in Steem）
- 减少交易费用（Eliminating Transaction Fees）
    - 费用问题（The Problem With Fees）
        - 小额支付不工作（Micropayments Don’t Work）
        - 费用是进入市场的壁垒（Fees are a Barrier to Entry）
        - 费用的调整（Changing Fees）
        - 女巫攻击（Sybil Attacks）
        - 完全保留和部分保留（Full Reserve vs Fractional Reserve）
    - 带宽代替小额支付渠道（Bandwidth Instead of Micropayment Channels）
        - 容量的影响（Impact of Capacity）
        - 费用比较（Comparison to Fees）
    - 账户创建（Account Creation）
    - 调整最低余额（Justifying Minimum Balances）
    - 费用的相对有效性（Effectiveness Relative to Fees）
    - 租赁、购买、时间共享（Renting vs. Buying vs. Time Sharing）
- 性能和可扩展性（Performance and Scalability）
    - Reddit规模（Reddit Scale）
- 初始分配和供应（Initial Allocation & Supply）
- 当前配置和供应（Current Allocation & Supply）
    - Token创建率的影响（Impact of Token Creation Rate）
- Steem的权利（The Power of Steem）
    - 没有小额支付，可选小费（No Micropayments, Tips Optional）
    - 价值在于链接（Value is in the Links）
    - 解决加密货币激活问题（Solving the Cryptocurrency Onboarding Problem）
    - 解决加密货币清算问题（Solving the Cryptocurrency Liquidation Problem）
    - 审查（Censorship）
    - 通过搜索引擎优化解决有机发现（Solving Organic Discovery via Search Engine Optimization）
    - 向基于区块链的署名转化（Shifting Toward Blockchain-based Attribution）
    - 用基于区块链的内容奖励替代广告（Replacing Advertising with Blockchain-based Content Rewards）
- 结论（Conclusion）

## 简介（Introduction）
用户生成的内容已为社交媒体公司的股东们创造了上亿美元的财富，例如Reddit、Facebook和Twitter。2014年，Reddit假设，如果每一个在reddit.com上发文、评论或投票等提供内容的人都获得公平份额的奖励，那么其平台将得到改进。Steem的目标是支持社交媒体和在线社区，将其大部分价值回报给那些为进入市场提供有价值的人，包括那些尚未参与任何加密货币经济的人。  

Steem的设计采用了很多关键原则：
- 最重要的原则是，每个参与投资的人都应该获得股份所有权、付款或债务作为回报。这一原则与所有创业公司相同，因为他们在创立初期和随后的融资过程中会分配股份。
- 第二个原则是，所有形式的资本都同样有价值。这意味着，那些为他人贡献自己的宝贵时间和注意力的人，和那些贡献自己的稀缺现金的人一样有价值。这是“汗水公平原则”(sweat equity principle)，这是以前的加密货币在提供服务的对象稍微多一点时就常常遇到困扰的一个概念。
- 第三个原则是社区生产产品，为其成员服务。这一原则的应用实例包括信用社、食品合作社和健康共享计划，只为社区成员提供服务而非向共享社区以外的人群出售产品或提供服务。

Steem社区向其成员提供以下服务：
1. 发掘新闻和评论的来源；
2. 为个性化问题提供优质答案的途径；
3. 提供与美元挂钩的稳定加密货币；
4. 支持自由支付；
5. 向其他成员提供上述服务相关的工作。

Steem有目的地对经济激励进行了重新调整，有可能为所有参与者创造更公平、更包容的结果，而不是像之前的社交媒体和加密货币平台那样。
本文将讨论现有的经济激励机制，并论证Steem的激励机制如何为大多数参与者带来更好的结果。  

> Collectively, user-generated content has created billions of dollars worth of value for the shareholders of social media companies, such as Reddit, Facebook, and Twitter. In 2014, Reddit hypothesized that its platform would be improved if everyone who contributed to reddit.com by posting stories, adding comments or voting were rewarded with a fair share in Reddit, Inc . Steem aims to support social media and online communities by returning much of its value to the people who provide valuable contributions by rewarding them with cryptocurrency, and through this process create a currency that is able to reach a broad market, including people who have yet to participate in any cryptocurrency economy. 
There are some key principles that have been used to guide the design of Steem. The most important principle is that everyone who contributes to a venture should receive pro-rata ownership, payment or debt from the venture. This principle is the same principle that is applied to all startups as they allocate shares at founding and during subsequent funding rounds.
The second principle is that all forms of capital are equally valuable. This means that those who contribute their scarce time and attention toward producing and curating content for others are just as valuable as those who contribute their scarce cash. This is the sweat equity principle and is a concept that prior cryptocurrencies have often had trouble providing to more than a few dozen individuals.
The third principle is that the community produces products to serve its members. This principle is exemplified by credit unions, food co-ops, and health sharing plans, which serve the members of their community rather than sell products or services to people outside the community.
The Steem community provides the following services to its members:
1, A source of curated news and commentary.
2, A means to get high quality answers to personalized questions.
3, A stable cryptocurrency pegged to the U.S. dollar.
4, Free payments.
5, Jobs providing above services to other members.  
Steem’s purposeful realignment of economic incentives has the potential to produce fairer and more inclusive results for everyone involved than the social media and cryptocurrency platforms that have gone before it. This paper will explore the existing economic incentives and demonstrate how Steem’s incentives may result in better outcomes for most participants.

#### 识别贡献（Recognizing Contribution）
Steem的设计宗旨是以解决社交媒体经济体中信息采用和货币化的主要障碍。我们的论点是，用于发展主要社交媒体平台的技术也可以用来引导加密货币的成功。加密货币带来的经济激励可以极大的促进新的社交媒体平台的发展。我们认为加密货币和社交媒体之间的协同作用会给  Steem在市场上带来强大的优势。  

Steem面临的挑战是推衍出一种对个人贡献内容进行评估的算法，能够得出大多数社区成员认同的对每一个贡献内容主观价值的公平评估。在一个完美的世界里，社区成员相互合作，对彼此的贡献进行评估并获得公平的奖励。而在现实世界中，算法的设计必须能够抵抗某些人故意操纵获益。任何滥用评分系统的行为都可能导致社区成员对经济体系的公平性失去信任。  

现有平台多数采用一用户一票原则运作。在这个环境中，排名可以被一种叫做“女巫攻击”的手段进行操纵，服务提供商必须主动识别并阻止拦截舞弊者。尽管唯一的奖励是网络流量或网络审查，人们已经试图操纵Reddit、Facebook和Twitter的评分算法。

Steem平台上的基本记账单位是STEEM，一种加密货币的Token（通证）。Steem的运行基础是1STEEM一票。在这种模式下，按照账户余额衡量，对平台贡献最大的个人对贡献评分的影响最大。此外，Steem只允许拥有Token的成员参与投票。在这种模式下，成员拥有足够的财务激励以实现Steem长期价值最大化的方式投票。

Steem的设计围绕一个相对简单的概念：每个人对社区的贡献都应该被认可。当自己的贡献获得认可时，他们才会继续贡献，社区才能不断发展。在一个社区内给予和接受的任何不平衡都是不可持续的。最终，给予者厌倦了支持获取者就会脱离社区。

我们面临的挑战是建立一个系统，能够识别需要哪些贡献，以及它们的相对价值，从而可以扩展支持无限的用户参与。

可以对贡献内容进行评估和提供奖励的一个可靠体系是自由市场。自由市场可以被看作是一个单独的社区，在这个社区中，每个人都可以彼此进行交易，通过收益和损失来分配奖励。市场体系会奖励那些向他人提供价值的人，惩罚那些消耗超过创造价值的人。自由市场支持许多不同的货币，而货币只是一种人人都能轻易交换的商品。

由于自由市场是一个经过验证的系统，因此试图建立一个自由市场体系，让内容消费者直接支付内容生产者是很有吸引力的。但是，对于内容创作者而言，直接付款是效率低下的，实际上也并不可行。大多数内容的价值相对于支付的认知、财务和机会成本而言是如此之低，以至于很少有读者选择支付。大量的免费选择意味着强制“付费门槛”将会驱使读者去其他地方。已经有一些尝试实现读者直接微支付到作者的每篇文章，但并没有广泛的应用。

Steem旨在通过经济模式来实现为各种内容贡献提供有效的微支付。读者不再需要决定他们是否想从自己口袋里掏钱，他们可以对内容进行投票，而Steem会用他们的选票来决定个人奖励。这意味着人们可以获得一个熟悉的、广泛使用的场景，不再面临传统微支付和打赏平台相关的认知、财务和机会成本。

社区成员的投票对Steem向贡献者准确分配奖励至关重要。因此，投票可以被视为一项重要贡献，它本身也值得奖励。一些平台，例如Slashdot，使用“meta-moderation”作为对诚信审核者进行排名和奖励的方式。Steem选择向那些为内容做出最大贡献的会员提供奖励，对投票人的奖励与向内容创建者支付的最终奖励成正比。

> Steem is designed from the ground up to address the major barriers to adoption and monetization of a social media based economy. Our thesis is that the same techniques used to grow major social media platforms can be used to bootstrap a successful cryptocurrency. Economic incentives enabled by cryptocurrency can dramatically facilitate the growth of a new social media platform. It is the synergy between cryptocurrency and social media that we believe may give Steem a powerful advantage in the market. 
The challenge faced by Steem is deriving an algorithm for scoring individual contributions that most community members consider to be a fair assessment of the subjective value of each contribution. In a perfect world, community members would cooperate to rate each other's contribution and derive a fair compensation. In the real world, algorithms must be designed in such a manner that they are resistant to intentional manipulation for profit. Any widespread abuse of the scoring system could cause community members to lose faith in the perceived fairness of the economic system. 
Existing platforms operate on a one-user, one-vote principle. This creates an environment where rankings can be manipulated by sybil attacks and the service providers must pro-actively identify and block abusers. People already attempt to manipulate the Reddit, Facebook, and Twitter scoring algorithms when the only reward is web traffic or censorship.
The fundamental unit of account on the Steem platform is STEEM, a crypto currency token.
Steem operates on the basis of one-STEEM, one-vote. Under this model, individuals who have contributed the most to the platform, as measured by their account balance, have the most influence over how contributions are scored. Furthermore, Steem only allows members to vote with STEEM when it is committed to a vesting schedule. Under this model, members have a financial incentive to vote in a way that maximises the long term value of their STEEM. 
Steem is designed around a relatively simple concept: everyone’s meaningful contribution to the community should be recognized for the value it adds. When people are recognized for their meaningful contributions, they continue contributing and the community grows. Any imbalance in the give and take within a community is unsustainable. Eventually the givers grow tired of supporting the takers and disengage from the community. 
The challenge is creating a system capable of identifying what contributions are needed and their relative worth in a way that can scale to an unbounded number of people. 
A proven system for evaluating and rewarding contributions is the free market. The free market can be viewed as a single community where everyone trades with one another and rewards are allocated by profit and loss. The market system rewards those who provide value to others and punishes those who consume more value than they produce. The free market supports many different currencies and money is simply a commodity that everyone finds easy to exchange. 
Since the free market is a proven system, it is tempting to try to create a free-market system where content consumers directly pay content producers. However, direct payment is inefficient and not really viable for content creation and curation. The value of most content is so low relative to the cognitive, financial, and opportunity costs associated with making a payment that few readers choose to tip. The abundance of free alternatives means that enforcing a ‘paywall’ will drive readers elsewhere. There have been several attempts to implement per-article micropayments from readers to authors, but none have become widespread. 
Steem is designed to enable effective micropayments for all kinds of contribution by changing the economic equation. Readers no longer have to decide whether or not they want to pay someone from their own pocket, instead they can vote content up or down and Steem will use their votes to determine individual rewards. This means that people are given a familiar and widely used interface and no longer face the cognitive, financial, and opportunity costs associated traditional micropayment and tipping platforms. Voting input from community members is critical for Steem to accurately allocate payments to contributors. 
Voting can therefore be viewed as a crucial contribution and worthy of rewards on its own. Some platforms, such as Slashdot, use meta-moderation as a way to rank and reward honest moderators. Steem chooses to reward those who contribute the most to the total promotion of a piece of content and rewards the voters proportional to the ultimate reward paid to the content creator.  
  
  
## 贡献方式（Ways to Contribute）
本节说明了Steem的概念以及如何奖励那些对Steem社区提供了有意义的、可计量贡献内容的会员。
> This section outlines the ideas behind Steem and its rewards for people who provide meaningful and measurable contributions to the Steem community.

#### 资本投入（Capital Contributions）
社区吸引资本贡献的两种方式：债务和所有权。持有社区所有权将在社区得到发展时获得收益，但在社区收缩时面临损失。那些债务的持有者，可以得到定量的利息保障，但是社区发展实现的利益与他们无关。这两种类型的资本贡献对社区的发展和货币价值都是有价值的。另外还有两种方式可以拥有所有权：交易和所有权。所有权是一种长期的承诺，在规定的短期之内不能出售。

Steem网络将这几种不同的资产类别称作“Steem”（STEEM）、“SteemPower”（SP）和“Steem Dollar”（SBD）。
 > There are two items a community can offer to attract capital: debt and ownership. Those who buy ownership profit when the community grows but lose if the community shrinks. Those who buy debt are guaranteed a certain amount of interest but do not get to participate in any profits realized by the growth of the community. Both types of capital contributions are valuable to the growth of the community and value of its currency. Additionally there are two ways ownership can be held: liquid and vesting. Vesting ownership makes a long-term commitment and cannot be sold for a minimum period of time.
The Steem network calls these different asset classes Steem (STEEM), Steem Power (SP), and Steem Dollars (SBD).

#### STEEM
Steem是这个链里最基础的账户单位。所有其他Token的价值都是从STEEM的价值衍生出来的。STEEM是一个流通货币，可以在任何一个交易平台买卖，也可以作为一种付款方式支付给其他用户。
> Steem is the fundamental unit of account on the Steem blockchain. All other tokens derive their value from the value of STEEM. STEEM is a liquid currency, and therefore can be bought or sold on exchanges, as well as transferred to other users as a form of payment.

#### Steem Power（SP）
创业公司需要长期的资金投入。那些投资初创公司的人要很长时间之后才能买卖他们持有的股权，实现获利。如果没有长期的资金支持，创业公司想通过出让更多股份吸引更多资金的时候，当前一轮的资金支持者想退出时，那么新资金支持者就会与前一轮资金支持者在竞争。精明的投资者希望他们的资金能够帮助公司成长，但是如果新的资金是交易给那些想要退出的原有资金支持者的话，那么这个公司价值得不到增长。

长期资金支持很重要，因为可以让社区有长期的规划。长期支持的股东们也会去为了长期发展而进行投票，而不是为了短期的资金回报。

在数字货币领域，投机者从一个数字货币跳到另一个数字货币，主要是基于预期的短期增长。Steem想要建设一个主要由拥有长远眼光的会员拥有和完全控制的社区。

用户可以把他们的STEEM放在一个13个星期的固定计划里，给用户提供一些更多的利益。任何Steem加入到这个13个星期的固定计划里都叫做SP。SP是不可以交易的，除非是通过自动循环的转换请求。这意味SP不能够轻易的在任何交易平台进行交易。

当用户对内容进行投票时，他们拥有的SP的数量和对奖励池分配的影响是成正比的。拥有更多SP的用户对奖励的分配有更大的影响。这意味着SP是一种能让它的持有者在Steem平台中获得权力的Token。

平台会给SP的持有者支付利息，每年15%的升值会作为利息，他们所获得的利息是与他们所持有的相对于所有用户的SP的数量成正比。

STEEM到SP的转化称之为“提升权限”，SP到STEEM的转化称之为“削弱权限”。SP转化STEEM是在用户提交“削弱权限”操作的一周之后开始返还，通过13周的平均每周支付返还完成。

> Start up companies require long-term capital commitment. Those who invest their money in a startup expect to wait years before they can sell their shares and realize their profits. Without long-term commitment, a startup seeking to raise additional capital through the sale of additional shares would be competing with existing shareholders looking to exit. Savvy investors want their capital contributions to grow the company, but growth cannot happen if the new capital is given away to those looking to exit.
There is significant value to having long-term commitment because it enables communities to make long-term plans. Long term commitment of stakeholders also causes them to vote for long-term growth rather than short-term pumps.
In the cryptocurrency space, speculators jump from cryptocurrency to cryptocurrency based mostly on which one is expected to have short-term growth. Steem wants to build a community that is mostly owned and entirely controlled by those with a long-term perspective.
Users are able to commit their STEEM to a thirteen week vesting schedule, providing them with additional benefits within the platform. STEEM that has been committed to a thirteen week vesting schedule is called Steem Power (SP). SP balances are non-transferrable and non-divisible except via the automatically recurring conversion requests. This means that SP cannot be easily traded on cryptocurrency exchanges.
When users vote on content, their influence over the distribution of the rewards pool is directly
proportional to the amount of SP that they have. Users with more SP have more influence on the distribution of rewards. This means that SP is an access token that grants its holders exclusive powers within the Steem platform.
SP holders are also paid interest on the balance of SP that remains vested. 15% of the yearly inflation is paid to SP holders as interest. The amount of the interest that they receive is directly proportional to the amount of SP they hold relative to the total amount of vested SP across all users.
Transferring from STEEM to SP is referred to as “powering up”, while transferring from SP to STEEM is referred to as “powering down.” SP that is powered down is returned to the user over a period of thirteen weeks, via 13 equal weekly payments, starting one week after the power down is initiated.

#### Steem Dollars（SBD）
成功的全球经济一个重要特征是稳定。在没有稳定性的情况下，世界各地的个人在从事商业和储蓄时，无法获得低认知成本。因为稳定性是非常重要的环节，所以SBD的研发是希望能够带给数字货币世界和用Steem网络的人带来稳定性。

Steem Dollars是由一种类似于可转换债券的机制创建的，它通常用于为初创公司提供资金。在创业公司中，可转换债券是短期债务工具，可以在未来的融资周期中根据确定的利率转换成所有权。基于区块链的Token可以看作是社区的所有权，而可转换债券可以被视为以任何其他商品或货币计价的债务。可转换债券的条款允许持有人以最少的通知，以公平的市场价格转换为支持令牌。创建可转换美元的Token可以使区块链Token持有者的回报最大化，增强其网络效应。

Steem Dollars被称为SBD，是steem blockchain dollars的缩写。创建SBD需要结合可靠的价格和防止滥用的规则。提供一个可靠的价格包括三个因素：最小化不正确feed的影响，最大化生产不正确feed的成本，尽量减少时间的重要性。

> Stability is an important feature of successful global economies. Without stability, individuals across the world could not have low cognitive costs while engaging in commerce and savings. Because stability is an important feature of successful economies, Steem Dollars were designed as an attempt to bring stability to the world of cryptocurrency and to the individuals who use the Steem network.
Steem Dollars are created by a mechanism similar to convertible notes, which are often used to fund startups. In the startup world, convertible notes are short-term debt instruments that can be converted to ownership at a rate determined in the future, typically during a future funding round. A blockchain based token can be viewed as ownership in the community whereas a convertible note can be viewed as a debt denominated in any other commodity or currency. The terms of the convertible note allow the holder to convert to the backing token with a minimum notice at the fair market price of the token. Creating token-convertible-dollars enables blockchains to grow their network effect while maximizing the return for token holders.
Steem Dollars are referred to with the symbol SBD, an acronym for Steem Blockchain Dollars. Creating SBD requires a combination of a reliable price feed, and rules to prevent abuse. Providing a reliable price feed involves three factors: minimizing the impact of an incorrect feed, maximizing the cost of producing an incorrect feed, and minimizing the importance of timing.

#### 减少虚假欺诈性Feeds（Minimizing Fraudulent Feeds）
> 特别解释feed：在这里feed流，直接翻译叫饲料，其实是把用户都比喻成爱吃东西得某种动物，不断的给他喂食，满足他的需求。简单说来，就是一种信息单元格，你也可以理解为某一个卡片、一段文字、视频、音频等等的信息单元。

SP持有人选举出一位代表（称为证人）来公布价格信息。假定当选的“证人”是被高质量Feed流的既得利益者所信任。通过支付报酬给“证人”，Steem创造了一种争夺Feed流生产权的市场竞争。Feed流生产者（平台作者）因为生产而得到的报酬越多，他们就越会因为发布虚假信息而损失更多。

给定一组受信任的和经过选举的Feed流生产者（平台作者），可以推衍出用于转换的实际价格，用作输入的中值。通过这种方式，如果任何少数的Feed流生产者（平台作者）产生了异常值，他们对实际中值的影响最小，实际中值仍然可信。

即使所有的Feed流生产者（平台作者）都是诚实的，大多数Feed流生产者（平台作者）也有可能受到超出他们控制的事件所影响。Steem网络的设计是能容忍中值Feed流的短期混乱，而社区则积极致力于纠正问题。一个例子是短期市场操纵可能需要一些时间去纠正。市场操纵很困难，而且要维持很长一段时间是很昂贵的。另一个例子是未能集中交易或交易发布数据的不良影响。

Steem利用3.5天时间的中值价格来避免短期价格波动因素。每小时对中值进行抽样。

只要价格供应的腐败持续不到一半的移动中值时间窗口，它将对转换价格产生影响是极小的。如果feed确实被破坏了，网络参与者将有机会在损坏的feed影响实际的转换价格之前，将腐败的Feed生产者（平台作者）排除在外。或许更重要的是，它给了Feed生产者一个机会，在他们的Feed影响价格之前，发现和纠正问题。

因为是3.5天的一个时间范围，社区会员可以有一天半的时间对产生的问题作出回应。

> SP holders elect individuals, called witnesses, to publish price feeds. The elected witnesses are presumably trusted by those who have a vested interest in the quality of the feed. By paying those who are elected, Steem creates market competition to earn the right to produce feeds. The more the feed producers are paid the more they have to lose by publishing false information.
Given a set of trusted and elected feed producers, the actual price used for conversions can be derived as the median of the feeds. In this way if any minority of individual feed producers produce outliers they have minimal impact on the actual median while still having the ability impact their reputation.
Even if all feed producers are honest, it is possible for the majority of feed producers to be impacted by events beyond their control. The Steem network is designed to tolerate short-term corruption of the median price feed while the community actively works to correct the issue. One example of an issue that may take some time to correct is short-term market manipulation. Market manipulation is difficult and expensive to maintain for long periods of time. Another example would be the failure of a centralized exchange or the corruption of the data published by the exchange.
Steem factors out short-term price fluctuations by using the median price over a period of three and a half days. The median published feed is sampled every hour on the hour.
As long as the price feed corruption lasts for less than half the moving median time window it will have minimal impact on the conversion price. In the event the feed does get corrupted, network participants will have an opportunity to vote-out corrupt feed producers before the corrupted feed can impact the actual conversion price. Perhaps more importantly, it gives feed producers an opportunity to detect and correct issues before their feeds start impacting the price.
With a three and a half day window, community members have approximately one and a half days to respond to any issues that come up.

#### 减轻时间攻击（Mitigating Timing Attacks）
市场参与者获得新信息的速度可以比3.5天中值转换的时间更快。这些信息可以使投机者盈利，代价是牺牲了社区的利益。如果Steem的价值突然增加，投机者可以用更低的旧价格转换SBD，然后极小风险的以更高的价格将Steem卖出。

Steem通过将所有的转换请求被延迟3天半的机制来平衡。这意味着在执行转换时，无论是交易员还是区块链都没有任何信息优势。

> Market participants have access to information faster than the blockchain’s three and a half day moving median conversion price can react. This information could be used to benefit of traders at the expense of the community. If there is a sudden increase in the value of STEEM traders could request conversion of their SBD at the old, lower price, and then sell the STEEM they receive a the new higher price with minimal risk.
Steem levels the playing field by requiring all conversion requests to be delayed for three and a half days. This means that neither the traders nor the blockchain has any information advantage regarding the price at the time the conversion is executed.

#### 减少滥用转换（Minimizing Abuse of Conversions）
如果人们可以在两个方向上自由转换，那么交易者就可以利用区块链转换速度进行大量交易而不改变其价格。那些看到价格大幅上涨的交易员将会以高价格(当风险最大的时候)转换为SBD，然后在价格回调之后再转换回来。Steem协议只允许人们从SBD转换为Steem而不是反过来，以此来保护社区免。

区块链决定如何和何时创建SBD，谁应该得到它。这使作为创作的速度稳定,消除了大多数投机途径。

> If people could freely convert in both directions then traders could take advantage of the blockchains conversion rates by trading large volumes without changing the price. Traders who see a massive run up in price would convert to SBD at the high price (when it is most risky) and then convert back after the correction. The Steem protocol protects the community from this kind of abuse by only allowing people to convert from SBD to STEEM and not the other way around.
The blockchain decides how and when to create SBD and who should get it. This keeps the rate of SBD creation stable and removes most avenues of abuse.

#### 可持续债务与股权比率（Sustainable Debt to Ownership Ratios）
如果Token在整个链里视为所有权的话，那么一个可转成Dollar的Token（token-convertible-dollar）可被理解成债务。如果负债率过高，整个货币就会变得不稳定。债务的转换可以显著增加Token的供应，从而在市场上以压低价格出售。后续交易需要发行更多Token。如果放任不管，这个体系就会崩溃，导致毫无价值的所有权和高额债务。债务与所有权比率越高，新投资者就越不愿意把资金投入。

STEEM价值的快速变化可以很大改变债务与所有权比率。Steem为了防止债务与所有权比率过高，如果债务水平超过10%，则通过SBD转换获得的STEEM数量减少。如果SBD的债务总额超过了整个STEEM市值的10%，区块链将自动减少通过转换产生的STEEM的数量，达到市场上限的10%，这将确保区块链永远不会超过10%的债务与所有权比率。

用于计算STEEM创建的百分比是基于供应量的，包括所有未完成的SBD和SP的STEEM值(由当前的rate / feed决定)。

> If a token is viewed as ownership in the whole supply of tokens, then a token-convertible-dollar can be viewed as debt. If the debt to ownership ratio gets too high the entire currency can become unstable. Debt conversions can dramatically increase the token supply, which in turn is sold on the market suppressing the price. Subsequent conversions require the issuance of even more tokens. Left unchecked the system can collapse leaving worthless ownership backing a mountain of debt. The higher the debt to ownership ratio becomes the less willing new investors are to bring capital to the table.
A rapid change in the value of STEEM can dramatically change the debt-to-ownership ratio. The blockchain prevents the debt-to-ownership ratio from getting too high, by reducing the amount of STEEM awarded through SBD conversions if the debt level were to exceed 10%. If the amount of SBD debt ever exceeds 10% of the total STEEM market cap, the blockchain will automatically reduce the amount of STEEM generated through conversions to a maximum of 10% of the market cap. This ensures that the blockchain will never have higher than a 10% debt-to-ownership ratio.
The percentage floors used to compute STEEM creation are based on the supply including the STEEM value of all outstanding SBD and SP (as determined by the current rate / feed).

#### 利息（Interest）
SBD像持有者支付利息。利率是由那些发布价格信息的人设定的，这样他们就可以适应不断变化的市场环境。所有的债务都会给贷款人带来风险。持有SBD而不赎回它的人实际上是在向社区提供一美元的价值。他们相信，将来某一时刻，有人会愿意以一美元的价格从他们手中购买SBD，或者会有投机者和投资者愿意购买他们将其转换成的股票。

当社区成员愿意持有SBD时，STEEM和SP持有者获得了优势。这种杠杆放大了增长的收益，同时也促进了增长。如果价格下跌，STEEM持有者确实会遭受更大的稀释。加密货币项目已经表明，通过增加用户基础来信任网络的收益，最终会给网络带来更多的价值，而不是在经济低迷时期可能出现的稀释。

>SBD pays holders interest. The interest rate is set by the same people who publish the price feed so that it can adapt to changing market conditions. All debt carries risk to the lender. Someone who holds SBD without redeeming it is effectively lending the community the value of a dollar. They are trusting that at some point in the future someone will be willing to buy the SBD from them for a dollar or that there will be speculators and investors willing to buy the STEEM they convert it into.
STEEM and SP holders gain leverage when members of the community are willing to hold SBD. This leverage amplifies the gains from growth while also contributing to growth. STEEM holders do suffer from increased dilution if the price falls. Cryptocurrency projects have shown that the gains from increasing the user base willing to trust the network with capital ultimately add more value to the network than any dilution that may occur during a downturn.

#### 制作价值供给（Setting Price Feeds）
精明的读者会认识到，有限供应的利益性资产，可能会比基础资产的价格更高或更低，这取决于相同资产赚取利息的其他机会。由于对一种与美元挂钩的资产支付了很高的利率，许多人将会抬高有限的SBD的供应，直到他们不再被估值为1美元。在经济学中，有一个理论叫三元悖论（Mundellian Trilemma），也称三难选择(The Impossible Trinity)，即不可能同时具备以下三个条件：
1.	汇率的稳定性
2.	资本的完全流动性
3.	货币政策的独立性

如果Steem的Feed生产者的目标是建立一个独立的货币政策，允许它创造并摧毁Steem Dollars，同时对利率进行完全控制，那么它们就会遇到问题。根据三元悖论理论，Steem Dollars要么需要限制资本流动，要么与美元有不稳定的汇率，要么对利率的控制有限。

Steem的Feed生产者主要关注的是在SBD和美元之间维持一个稳定的一对一的转换。任何时候SBD持续交易超过$1.00美元的利息支付必须停止。在一个债券的0%利率仍然需要溢价的市场中，可以肯定地说，市场愿意提供比社区愿意承担的债务更多的信贷。如果这种情况发生，SBD的价值将超过1.00美元，而且社区也不可能不收取负利率。

如果债务与所有权比率较低，而SBD的交易价格低于1.00美元，则应增加利率。这将鼓励更多的人持有他们的SBD并支持价格。

如果SBD的交易价格低于1美元，而债务与所有权比率很高，那么feed应该向上调整，给每个SBD提供更多的STEEM。这将增加对SBD的需求，同时也降低了债务与所有权比率，并使SBD与美元等值。

假设STEEM的价值增长快于STEEM创建新的SBD，那么债务与所有者的比率应该保持在目标比率之下，而利息会给每个人带来好处。如果网络的价值是持平或下降的，那么任何提供的利息只会使债务与所有权比率更差。

实际上，Feed生产者肩负着制定货币政策的责任，目的是为了维持与美元的稳定挂钩。滥用这种权力会损害STEEM的价值，因此SP持有者明智地投票给那些可以根据上面列出的规则来调整价格和利率的证人。

如果债务与所有权比率过高，市场参与者选择避免转换请求，则应调整饲料价格，以提高为转换SBD而支付的利率。

对利率政策和/或对STEEM/SBD转化率的任何溢价/折扣的改变，应该是对长期平均偏差的缓慢而慎重的反应，而不是试图对短期市场状况作出反应。

我们相信，这些规则将使市场参与者相信，他们不可能以1.00美元的价格持有SBD而蒙受损失。我们完全预计，在正常市场情况下，SBD的交易区间在0.95 - 1.05美元之间。

> Astute readers will recognize that an interest bearing asset of limited supply may trade higher or lower than the underlying asset depending upon other opportunities to earn interest on the same asset. With a high interest rate paid on an asset pegged to the US dollar many people will bid up the limited supply of Steem Dollars until they are no longer valued at $1. In economics there is a principle known as the Impossible Trinity which states that it is impossible to have all three of the following at the same time:
> 1. A stable exchange rate
> 2. Free capital movement
> 3. An independent monetary policy  
>  
> If Steem feed producers aim to have an independent monetary policy allowing it to create and destroy Steem Dollars while simultaneously having full control over the interest rate then they will encounter problems. The Impossible Trinity says that Steem Dollars either need to restrict capital movement, have an unstable exchange rate with the dollar, or have limited control over the interest rate.
The primary concern of Steem feed producers is to maintain a stable one-to-one conversion between SBD and the U.S. Dollar (USD). Any time SBD is consistently trading above $1.00 USD interest payments must be stopped. In a market where 0% interest on debt still demands a premium, it is safe to say the market is willing to extend more credit than the debt the community is willing to take on. If this happens a SBD will be valued at more than $1.00 and there is little the community can do without charging negative interest rates.
If the debt-to-ownership ratio is low and SBD is trading for less than $1.00, then the interest rate should be increased. This will encourage more people to hold their SBD and support the price.
If SBD trades for less than $1.00 USD and the debt-to-ownership ratio is high, then the feeds should be adjusted upward give more STEEM per SBD. This will increase demand for SBD while also reducing the debt-to-ownership ratio and returning SBD to parity with USD.
Assuming the value of STEEM is growing faster than Steem is creating new SBD, the debt-to-ownership ratio should remain under the target ratio and the interest offered benefits everyone. If the value of the network is flat or falling, then any interest offered will only make the debt-to-ownership ratio worse.
In effect, feed producers are entrusted with the responsibility of setting monetary policy for the purpose of maintaining a stable peg to the USD. Abuse of this power can harm the value of STEEM so SP holders are wise to vote for witnesses that can be counted on to adjust the price feed and interest rates according to the rules outlined above.
If the debt-to-ownership ratio gets dangerously high and market participants choose to avoid conversion requests, then the feed should be adjusted to increase the rate at which STEEM paid for converting SBD.
Changes to the interest rate policy and/or any premiums/discounts on the STEEM/SBD conversion rate should be a slow and measured response to long-term average deviations rather than attempting to respond to short-term market conditions.
It is our belief that these rules will give market participants confidence that they are unlikely lose money by holding SBD purchased at a price of $1.00. We fully expect there to be a narrow trading range between $0.95 and $1.05 for SBD under normal market conditions.

## 主观贡献（Subjective Contributions）
对工作的主观证明提出了一种分配货币的替代方法，这种方法可以提高对采矿等工作系统的完全客观证明。货币实施主观证明的应用比任何工作制度的客观证据都要广泛得多，因为它们可以应用于建立一个有充分明确目的的概念的社区。当个人加入一个社区时，他们会购买一套特定的信仰，并投票支持社区的价值观或目的。

实际上，评估工作的标准是完全主观的，而且它的定义也存在于源代码本身之外。一个社区可能希望奖励艺术家、另一个诗人和另一个喜剧演员。其他社区可能选择奖励慈善事业或帮助推进政治议程。

每一种货币的价值取决于特定社区内对影响力的需求，以及市场认为每个社区能获得多大的影响力。与以前的系统不同，主观的工作证明使一个社区能够共同资助任何它认为有价值的东西的发展，并使以前不赚钱的时间货币化。

> Subjective Proof of Work presents an alternative approach to distributing a currency that improves upon fully objective Proof of Work systems such as mining. The applications of a currency implementing subjective proof of work are far wider than any objective proof of work system because they can be applied to build a community around any concept that has a sufficiently defined purpose. When individuals join a community they buy into a particular set of beliefs and can vote to reinforce the community values or purpose.
In effect, the criteria by which work is evaluated is completely subjective and its definition lives outside the source code itself. One community may wish to reward artists, another poets, and another comedians. Other communities may choose to reward charitable causes or help advance political agendas.
The value each currency achieves depends upon the demand for influence within a particular community and how large the market believes each community can get. Unlike prior systems, subjective proof of work enables a community to collectively fund the development of whatever it finds valuable and enables the monetization of previously non monetizable time.

#### 分配货币（Distributing Currency）
人们可以通过两种方式参与加密货币社区:他们可以购买，或者他们可以工作。在这两种情况下，用户都在增加货币的价值，然而，绝大多数人的空闲时间都比他们的闲钱多。想象一下，在一个没有实际现金但却有足够时间的贫困社区，引导一种货币的目标是什么。如果人们可以通过为彼此工作而赚钱，那么他们将通过一个公平的会计/货币体系促进相互交流。

将一种货币分配给尽可能多的人，这种方式通常被认为是公平的，是一项具有挑战性的任务。一个客观的计算机算法可以完全评估的任务在本质上是有限的，总的来说，它的外部好处是有限的。在BTC挖矿中，它可以产生专门的硬件，并导致人们投入时间开发更高效的算法。它甚至可以帮助找到质数，但这些东西都不能给社会或货币持有群体提供有意义的价值。更重要的是，规模经济和市场力量最终将排除所有人，但专家参与了这种分配。最终，基于计算的挖掘是另一种购买方式，因为它需要钱来支付电费，或者开发完成工作所需的硬件。

为了让每个人都有平等的机会参与和赚取货币，必须给他们一个工作的机会。挑战在于如何判断个人提供的工作的相对质量和数量，以及如何有效地分配给数百万用户的报酬。这需要引入可扩展的投票过程。特别是，它要求分配资金的权力必须尽可能地分散。

奖励数百万用户的第一步是承诺分配一定数量的货币，无论实际做了多少工作或用户如何投票。这就改变了“我们应该付款吗?”“我们该付给谁?”向市场发出的信号是，资金正在被分配，并被拍卖给那些“出价”最多的人。这类似于比特币承诺将50BTC奖励给找到最困难哈希的人。就像比特币一样，所有的工作都必须是付出代价才有回报，而对于未来要做的工作，任何事情都不应该进行投机。

下一步是奖励每一个做任何事情的人，哪怕是只有一点积极的东西。这是通过对所有工作进行排序并按比例分配来完成的。市场越有竞争力，就越难(质量或数量)获得相同的回报。

> There are two ways people can get involved with a crypto-currency community: they can buy in , or they can work in . In both cases users are adding value to the currency, however, the vast majority of people have more free time than they do spare cash . Imagine the goal of bootstrapping a currency in a poor community with no actual cash but plenty of time . If people can earn money by working for one another then they will bootstrap value through mutual exchange facilitated by a fair accounting/currency system.
Distributing a currency to as many people as possible in a manner that is generally perceived as fair is a challenging task. The tasks that can be entirely evaluated by an objective computer algorithm are limited in nature and generally speaking have limited positive external benefits. In the case of Bitcoin-style mining, it can result in the production of specialized hardware and cause people to invest time developing more efficient algorithms. It may even help find prime numbers, but none of these things provide meaningful value to society or the currency holding community at large. More importantly, economies of scale and market forces will end up excluding everyone but experts from participating in this kind of distribution. Ultimately, computation-based mining is just another way of buying in because it requires money to pay the electric bill or the development of hardware necessary to do the work.
In order to give everyone an equal opportunity to get involved and earn the currency people must be given an opportunity to work. The challenge is how to judge the relative quality and quantity of work that individuals provide and to do so in a way that efficiently allocates rewards to millions of users. This requires the introduction of a scalable voting process. In particular it requires that authority to allocate funds must be as distributed and decentralized as possible.
The first step in rewarding millions of users is to commit to distributing a fixed amount of currency regardless of how much work is actually done or how users vote. This changes the question from being “ Should we pay? ” to “ Whom should we pay? ” and signals to the market that money is being distributed and is being auctioned off to whoever “bids” the most work . This is similar to Bitcoin committing to award 50 BTC to whoever finds the most difficult hashes. Like Bitcoin, all work must be done prior-to payout and nothing should be paid speculatively on the promise to do work in the future.
The next step is to reward everyone who does anything even remotely positive with something . This is accomplished by ranking all work done and distributing proportionally to its value. The more competitive the market becomes, the more difficult (higher quality or quantity) it becomes to earn the same payout.

## 对货币分配进行投票（Voting on Distribution of Currency）
假设有固定资金分配，而那些对货币未来价值和效用有长期投资兴趣的人必须决定如何分配这些货币。每一个投资者都投了自己的票，谁做了最好的工作，在一天结束的时候，那一天的可用资金被分成了比例，因此一个人即使只有一份投票也会获得奖励。

不成熟的投票流程会产生“囚徒困境”，会产生每一名投票者为自己投票的诱因，代价是损害更大的社区利益。如果每个投票者都只为自己投票，最终将没有可分配的货币，货币也无法带来相应的网络效应。另一方面，如果只有一名投票者违反规则，那么只有该投票者取得不应得利益，同时对货币的整理价值产生的影响极小。

> Assume there is a fixed amount of money to distribute, and that those who have a long-term vested interest in the future value and utility of the currency are the ones who must decide how to allocate it. Every vesting user casts their votes on who did the best work and at the end of the day the available money for that day is divided proportional to the votes such that everyone with even one net positive vote gets something.
The naive voting process creates a N-Person Prisoner’s Dilemma5 whereby each individual voter has incentive to vote for themselves at the expense of the larger community goal. If every voter defects by voting for themselves then no currency will end up distributed and the currency as a whole will fail to gain network effect. On the other hand, if only one voter defects then that voter would win undeserved profits while having minimal effect on the overall value of the currency.

#### 滥用投票权（Voting Abuse）
不管一个人拥有多少钱，总有很多人拥有相似的财富。即使是最富有的人，也很少有比下一对最富有的人加起来还要多。此外，那些在社区中有大笔投资的人也会因为试图为自己的投票系统而损失最大的损失。这类似于公司的CEO决定停止支付工资，因此可以将所有利润装进自己口袋一样。但是每个人都会离开，为其他公司工作，然后公司将变得分文不值，CEO最终破产而不是富有。

幸运的是，任何获得大量投票的工作也要经受最严格的审查(宣传)。通过增加否决票，消除了很多较小利益相关者串通进行团体投票，或较大利益相关者滥用投票权的可能。此外，当较大的利益相关者滥用投票权时，会由于货币的价值由于舞弊下降而遭受的损失更大。事实上，诚信的较大利益相关者可能在治理舞弊和利用反对票方面比较小利益相关者投票更有效。

使用负投票权来防止人们滥用这个系统，利用了许多人在被认为是一个人以牺牲其他人利益为代价的时候所拥有的螃蟹思维。螃蟹思维通常指的是目光短浅的人把好人打倒在地，但这也是让好人把坏人打倒的原因。唯一的“问题”是当人们错误地认为别人在为别人的花费而获利时。

> Regardless of how much money any one individual has, there are always many other individuals with similar wealth. Even the wealthiest individual rarely has much more than the next couple wealthiest combined. Furthermore, those who have a large investment in a community also have the most to lose by attempting to game the voting system for themselves. It would be like the CEO of a company deciding to stop paying salaries so he could pocket all of the profits. Everyone would leave to work for other companies and the company would become worthless, leaving the CEO bankrupt rather than wealthy.
Fortunately, any work that is getting a large concentration of votes is also gaining the most scrutiny (publicity). Through the addition of negative-voting it is possible for many smaller stakeholders to nullify the voting power of collusive groups or defecting large stakeholders. Furthermore, large-stakeholders have more to lose if the currency falls in value due to abuse than they might gain by voting for themselves. In fact, honest large stakeholders are likely to be more effective by policing abuse and using negative voting than they would be by voting for smaller contributions.
The use of negative-voting to keep people from abusing the system leverages the crab mentality that many people have when it is perceived that one individual is profiting at the expense of everyone else. While crab mentality normally refers to short-sighted people keeping good people down, it is also what allows good people to keep bad people down. The only “problem” with crab mentality is when people wrongly believe someone is profiting at everyone else's expense.

> ###### 螃蟹桶的故事（The Story of the Crab Bucket）
> 有个人在沙滩上散步，看到另一个人在岸边钓鱼，身边放着一个装诱饵的桶。走近之后，看到桶上并没有盖子，里面装了很多活的螃蟹。
“你为什么不盖上诱饵桶，免得螃蟹跑掉？”他问道。
“这个你就不知道了。”那人回答，“如果桶里只有一只螃蟹，它肯定会很快就能爬出来。但是，桶里有很多螃蟹时，如果有一只努力沿着桶壁向上爬，其余的会抓住它，把它拉下来，因此它也遭受与其余同伴们同样的命运。”
人类也一样。如果有人尝试做某些不一样的事情，获得更好的等级，提高自己，从自己的环境里逃出去，或者有远大的梦想，其他人就会尝试把他拖回来，也遭受与其余人同样的命运。
> 
> A man was walking along the beach and saw another man fishing in the surf with a
bait bucket beside him. As he drew closer, he saw that the bait bucket had no lid and
had live crabs inside.
"Why don't you cover your bait bucket so the crabs won't escape?", he said.
"You don't understand.", the man replied, "If there is one crab in the bucket it would
surely crawl out very quickly. However, when there are many crabs in the bucket, if
one tries to crawl up the side, the others grab hold of it and pull it back down so that
it will share the same fate as the rest of them."
So it is with people. If one tries to do something different, get better grades, improve
herself, escape her environment, or dream big dreams, other people will try to drag
her back down to share their fate.

消除“舞弊”是不可能的，也不应当成为目标。即使是那些试图在这个系统上“舞弊”的人仍然在工作。他们在舞弊或串通方向尝试成功获得的任何报酬，至少在货币分配目的上与传统的BTC采矿或通过矿池完成联合采矿一样，是有价值的。必须的工作是确保舞弊不会变得猖獗，以免削弱人们为支持社区和货币而进行真正工作的动机。

建设社区货币的目标是“在桶里获得更多的螃蟹”。而采取严厉措施消除所有“舞弊”，就像试图在桶上放个盖子来防止有些螃蟹逃脱，其代价是使得向桶里增加新的螃蟹变得更加困难。其实只要让桶壁变得光滑和给其他螃蟹足够的力量防止其他的逃脱就足够了。

> Eliminating “abuse” is not possible and shouldn’t be the goal. Even those who are attempting to “abuse” the system are still doing work. Any compensation they get for their successful attempts at abuse or collusion is at least as valuable for the purpose of distributing the currency as the make-work system employed by traditional Bitcoin mining or the collusive mining done via mining pools. All that is necessary is to ensure that abuse isn’t so rampant that it undermines the incentive to do real work in support of the community and its currency.
The goal of building a community currency is to get more “crabs in the bucket”. Going to extreme measures to eliminate all abuse is like attempting to put a lid on the bucket to prevent a few crabs from escaping and comes at the expense of making it harder to add new crabs to the bucket. It is sufficient to make the walls slippery and give the other crabs sufficient power to prevent others from escaping.


未完待续...
