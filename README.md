# Steem白皮书中文版 & 中英对照版
> 根据自己理解进行一次可读化的翻译。

### Steem
基于区块链的激励式公共内容平台。
> An incentivized, blockchain-based, public content platform.
August 2017

#### 摘要 - Abstract
Steem是一个支持社区建设与加密货币奖励社交互动的区块链。Steem将社交媒体、加密货币及社区建设相结合。鼓励参与任何社区、货币或自由市场经济的一个重要关键是：公正的会计制度，它将始终反映着每个人的贡献。Steem是第一个试图准确和透明的奖励无数为社区做出主观贡献者的加密货币。

> Steem is a blockchain database that supports community building and social interaction
with cryptocurrency rewards. Steem combines concepts from social media with lessons
learned from building cryptocurrencies and their communities. An important key to
inspiring participation in any community, currency or free market economy is a fair
accounting system that consistently reflects each person's contribution. Steem is the first
cryptocurrency that attempts to accurately and transparently reward an unbounded
number of individuals who make subjective contributions to its community.

#### 目录 - Table of Contents
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

#### 简介（Introduction）
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

未完待续...
