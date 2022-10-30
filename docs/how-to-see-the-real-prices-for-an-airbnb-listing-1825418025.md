# 如何查看 Airbnb 房源的真实价格

> 原文:[https://life hacker . com/how-to-see-the-real-prices-for-an-Airbnb-listing-1825418025](https://lifehacker.com/how-to-see-the-real-prices-for-an-airbnb-listing-1825418025)

[Airbnb](https://www.airbnb.com/) ，你的 UI 太烂了。我说的不是即将到来的假期我可以租的漂亮的房子和公寓的图片和展示；我说的是价格。当我查看房源时，我希望看到实际的每日价格——费用和一切都包含在每日平均价格中，因为我使用 Airbnb 正是因为我试图保持在一定的预算内。

Watch

换句话说，在 Airbnb 上找到一个价格刚好低于我承受范围的好地方，却眼睁睁地看着它飙升到超出我每晚想要花费的价格，这是很烦人的，因为在你预订一个地方之前，所有的杂费都被收取了。

这肯定是大卫的事情，因为大卫·索耶显然也有同样的抱怨——只是，他决定创建一个浏览器扩展，向你显示 Airbnb 的真实每日价格，在你预订之前，某个位置的费用会平均计入每日价格，而不是只是咧嘴笑着和 [处理它](http://gph.is/29j29Rz) 。你现在可以获得 [Chrome](https://chrome.google.com/webstore/detail/airbnb-price-per-night-co/lijeilcglmadpkbengpkfnkpmcehecfe) 和 [Firefox](https://addons.mozilla.org/en-US/firefox/addon/airbnb-price-per-night-correct/) 的扩展，但是有几个重要的注意事项。

首先，这个扩展只有当你在一个常规列表的预订页面时才起作用。在输入入住和退房日期之前，您会一直看到旧价格。当你这样做时，租赁星级以上的价格会更新，显示现在“包括费用”,并带有一个大大的勾号——你不会错过的。

其次，这一扩展似乎还不适用于 Airbnb 的“Airbnb Plus”房源。如果你在寻找皇家待遇，你只能自己计算每日价格，直到 Sawyer 发布扩展的更新(咳咳)。

最后，当你在一个列表的预订页面上时，扩展*只对*有效。当你浏览潜在的住宿地点时，如果所有地点的费用都计入价格，那绝对会令人惊讶，但这似乎有一些技术限制，正如 Sawyer 在 Reddit 上解释的 [:](https://www.reddit.com/r/AirBnB/comments/7lrnhf/i_built_a_chrome_extension_that_shows_you_the/)

> “很大程度上，主要原因是我必须依靠 Airbnb 的内部 API 来计算一次旅行的总价格，我觉得 Airbnb 可能会限制我的价格，因为当属性列表发生变化时，我可能会提出一堆请求。此外，如果他们要改变请求或响应的内容，使用他们的内部 API 很容易破坏扩展。
> 
> 我也不是 100%确定我能单独通过 API 调用一路到达那里。他们可能会用列表页面的 HTML 有效负载发送计算价格所需的其他值，这样也会增加很多复杂性。
> 
> 此外，我想我的思想不太关注“这能做到吗？”更多关于“当 Airbnb 改变一些东西时，维护/更新会有多糟糕？”当构建一个改变网页内容的扩展时，你的主要敌人是从你下面被改变的页面/代码结构，所以构建可靠性是我的一个很大的关注点。"

尽管 Sawyer 的扩展很小，并且在实用性上有一点限制，但它仍然是一个避免使用计算器来计算潜在列表的真实日费率的好方法。如果 Airbnb 正在阅读这篇文章——你们完全可以让这种定价魔法在你们这边发生，对吗？