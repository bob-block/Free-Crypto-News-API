# Free-Crypto-News-API

Since the cryptocurrency market is a dynamic one, with rates fluctuating by the second. Moreover, new currencies pop up all of the time, and investors and traders need to stay on top of the information. This is where Crypto News APIs come in.
A crypto news API is a REST API framework built on JSON that uses machine learning and NLP (Natural Language Processing) to identify relevant news sources based on your search criteria.

Block.cc is a professional cryptocurrency information service platform that provides cryptocurrency quotes, data, information, and high-performance RESTful JSON endpoints designed to meet the mission-critical demands of application developers, blockchain enthusiasts, cryptocurrency investors, and enterprise business platforms. Included 500+ exchanges, 10,000+ currencies, 28,000+ trading pairs, and 1000+ business users. It covers multi-dimensional data such as real-time price, historical transactions, currency information, K-line data, legal currency exchange rate, transaction depth, news flash, and block data.

Example request:
（1）Get Exchange Announcement List

curl -X GET \
  'https://data.block.cc/api/v3/announcements?locale=zh_CN'

Response:

 [
  {
    "title": "关于杠杆交易上线LTC/USDT、EOS/USDT、TRX/USDT的公告（1220）",
    "content": "尊敬的用户： \n\n\n BiKi平台将于2019年12月20日18:00开放LTC/USDT、EOS/USDT、TRX/USDT杠杆交易. \n\n  \n\n提示：\n 1、合理操作杠杆交易,可以提高收益.但同时考虑到加密货币市场目前的波动性,它也会为交易者带来更大的风险.\n 2、杠杆交易受市场风险、波动性和复杂性的影响较大,请您务必充分了解杠杆交易的风险后审慎使用,BiKi平台不对因杠杆交易造成的损失负责.\n  \n 感谢您对BiKi平台的支持,BiKi团队期待您的宝贵意见.\n BiKi团队\n 2019-12-20",
    "timestamp": 1576811020489,
    "importance": false,
    "url": "https://m.block.cc/news/5dfc3a0cc3af0a649f3f4563",
    "market": "bikicoin",
    "sourceUrl": "https://www.biki.com/noticeInfo/2007",
    "images": []
  },
  {
    "title": "Binance战略投资FTX并上市FTX Token（FTT）",
    "content": "亲爱的用户： \n\nBinance已完成对FTX的战略投资（投资详情）,现已上线FTX Token（FTT）,开通FTT/BNB、FTT/BTC、FTT/USDT 交易市场,邀您体验！FTT充值通道现已开放,立即充值. \n\nFTT的上币费用为0 BNB. \n\n声明：Binance已从对FTX的投资中获得了一部分FTT代币. 其中绝大多数FTT锁定期为两年. 我们致力于帮助FTT和FTX生态系统实现长期,可持续的发展. \n\n规则说明： \n\n- 关于FTX Token (FTT)\n- 费率说明\n- 交易规则 \n\n风险提示：数字货币是一种高风险的投资方式,请投资者谨慎购买,并注意投资风险.Binance会遴选优质币种,但不对投资行为承担担保、赔偿等责任. \n\n  \n\n感谢您对Binance的支持！ \n\n  \n\nBinance团队 \n\n2019年12月20日 \n\n  \n\nBinance社群 \n\n微博： https://weibo.com/u/7336825507  \n\nTelegram： https://t.me/BinanceChinese \n\nFacebook： https://www.facebook.com/BinanceChinese \n\nTwitter： https://twitter.com/binance",
    "timestamp": 1576810511000,
    "importance": false,
    "url": "https://m.block.cc/news/5dfc3a03c3af0a649f3f4416",
    "market": "binance",
    "sourceUrl": "https://binance.zendesk.com/hc/zh-cn/articles/360038147271-Binance%E6%88%98%E7%95%A5%E6%8A%95%E8%B5%84FTX%E5%B9%B6%E4%B8%8A%E5%B8%82FTX-Token-FTT-",
    "images": []
  }
]

（2）Get Briefs

curl -X GET \
  'https://data.block.cc/api/v3/briefs?locale=zh_CN'

Response:

 [
  {
    "images": [],
    "datetime": 1576477950000,
    "importance": false,
    "source": "金色财经",
    "title": "亿利集团董事长王文彪：要将区块链治沙模式推广到全世界",
    "content": "12月16日,IFIC全球金融科技创新峰会·东京站正式开幕.亿利资源集团董事长,库布齐沙漠治理的带头人王文彪在IFIC TOKYO开场致辞中表示,亿利集团在30余年的治理了库布其沙漠,我们的治理模式已经可以在全中国推广.区块链技术的集成应用在新的技术革新和产业变革中起着重要作用,我们想用区块链把沙漠治理模式带到全世界,向世界推广,为全人类做些贡献,做区块链公益.在此,希望日本的朋友到沙漠考察访问,将公益基金和区块链相连接,所投入的资金用来促进环境的发展,让全世界人知道怎样运用区块链使沙漠变成良田,达到可持续发展.",
    "url": "https://m.block.cc/news/5df724fe07a014563b8269c0"
  },
  {
    "images": [],
    "datetime": 1576477582000,
    "importance": false,
    "source": "小葱",
    "title": "工信部将从推动云计算与区块链等技术融合创新等入手推动云计算产业快速发展",
    "content": "工信部信软司副司长董大健表示,下一步,工信部将从五方面入手推动云计算产业快速发展.一是持续优化发展环境,规范云计算市场,培育龙头骨干企业；二是加快突破核心技术,加快云计算在自主基础软硬件平台上的适配迁移,推动云计算以5G、工业互联网、大数据、人工智能、区块链等技术融合创新；三是深入推动企业上云应用云；四是完善云计算的标准体系；五是打造安全保障体系.（c114）",
    "url": "https://m.block.cc/news/5df7238e07a014563b8269b4"
  }
]


（3）Get SocialMedia List

curl -X GET \
  'https://data.block.cc/api/v3/social_media?source=TWITTER'

Response:

[
  {
    "id": "1264806231472046080",
    "source": "TWITTER",
    "content": "The ability to recognize humor is a defining characteristic of intelligence.\n\nI use it constantly to cull my followers by placing the burden of culling upon themselves.",
    "images": [],
    "userId": "961445378",
    "avatar": "https://mifengcha.oss-cn-beijing.aliyuncs.com/static/twitter/screen_name/officialmcafee.jpg",
    "screenName": "officialmcafee",
    "timestamp": 1590388279000,
    "retweeted": false,
    "retweet": null
  },
  {
    "id": "1264805947861536771",
    "source": "TWITTER",
    "content": "⚡ @cartesiproject Listing + Contest ⚡\n\n$CTSI/USDT trading starts today at 5 PM IST on #WazirX.\n\nWe're giving away 378 #CTSI worth ₹1,000 each to 5 lucky people who:\n\n1. Retweet this tweet\n2. Reply to this tweet &amp; mention 3 friends in the reply\n\nValid for 24 hrs! https://t.co/MIhccc43AI",
    "images": [
      "https://mifengcha.oss-cn-beijing.aliyuncs.com/static/twitter/media/bdc36e0a6a2ad8f6be9bcabf3dead476.jpg"
    ],
    "userId": "955744720092835841",
    "avatar": "https://mifengcha.oss-cn-beijing.aliyuncs.com/static/twitter/screen_name/WazirXIndia.jpg",
    "screenName": "WazirXIndia",
    "timestamp": 1590388211000,
    "retweeted": false,
    "retweet": null
  }
]


Conclusion

Crypto News API is a powerful and flexible tool designed to provide users with real-time, comprehensive, and in-depth analysis capabilities, and provide more investors with a market forecast.
