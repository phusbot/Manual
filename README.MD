CloudGate Manual
==========

基于|CloudGate|https://github.com/BurpSuite/Manual|修改的规则，本人目前使用Shadowrocket，所以只修改了Shadowrocket规则。

修改目的：因为我的服务器屏蔽了国内的服务，使用原规则时发现新浪微博用不了，因原规则把新浪的域名也添加到代理规则里。

修改处：将`sina.com`修改为直连模式，屏蔽`umeng.com`后缀，删除`Rewrite=>Old_Rule_WebSite_Jump`。

规则地址 https://raw.githubusercontent.com/phusbot/Manual/master/Shadowrocket.Conf
