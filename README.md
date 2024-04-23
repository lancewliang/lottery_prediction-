# 彩票预测系统
    我在少年时期一个亲戚对彩票有执着的兴趣，当时就为其开发一个彩票的筛选程序。以及长大后亲戚因为彩票而输了很多钱导致家庭产生了重大的危机。这个项目的初衷并不是赚钱，对AI技术的尝试以及对彩票问题的一种探索。完成后我想把他公开给我的亲戚，给他们一个惊喜吧。相比彩票我觉得这些技术用于股票可能实用性更大一些。由于我是一个中文开发者所以我的底稿会用中文书写，然后翻译成英文。readme中我会将主要的设计思路记录下来，我会用更加通俗的方式来解释我的想法，不要和我讨论学术。那些希望通过本项目赚钱的可以离开了，娱乐性质的朋友是可以考虑使用或者继续开发下去。我也将会把这个项目变成一个有趣的网站放在公网使用（如果能赚一些广告或者捐助那就更好了，希望能把设备和网络费用给维持下来）。
    彩票的预测本来就是一个随机和运气以及博弈问题。我将方面讲述这个问题需要面对那些不可控的因素。
    * 所有的数学公式都不能准确的预测随机问题
    * 随机问题带来了运气这个因素，而运气每个人又不一样，为什么小概率时间会发生在你身上呢？
    * 贩卖彩票的机构是否本身就作弊，避免了中奖的小概率事件

    那么如何预测彩票呢？在说我的实现思路之前需要先了解下大爷们是怎么选彩票的，在论坛中瞎逛几年发现几种思路：
    *瞎猜杀号法，各种奇怪的规则杀号。用上期的首尾和除以3的得数视为杀码，注意取整。这些规则需要对历史数据进行统计，可能有用，我们可以测试这些规则，哪些还有用，我们可以考虑使用。
    *看图选号法，根据连续出现的数据组合，绘制成图形进行选号，这个和股票k线路有点类似，看不懂果断放弃。
    *基于数学特性数据分布维度的选号规则，单双数，数字和，数字分布分类，连续性，离散性等。这种数据的维度特征作为筛选数字非常有用，因此我将保留这些维度使用。
    *基于历史数据的数字出现热度来杀号或者选号。最近7次，出现了3次的数字要杀掉等等。这个其实也可以作为一种特征来看待，需要保留这种特征。
    *选学选号法，生日啦，天气啦，八字，占卜拉，纯靠大自然力量来选号。

    
    
     




