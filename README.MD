CloudGate Manual
==========

基于[CloudGate](https://github.com/BurpSuite/Manual)修改的规则，本人目前使用Shadowrocket，所以只修改了Shadowrocket规则。

修改目的：因为我的服务器屏蔽了国内的服务（[项目地址](https://github.com/phusbot/ss-iptables-blockade)），使用原规则时发现新浪微博用不了，因原规则把新浪的域名也添加到代理规则里。

修改处：将`sina.com`和`baidu.jp`修改为直连模式，新增`360.cn`为直连，屏蔽`umeng.com`后缀，删除`Rewrite=>Old_Rule_WebSite_Jump`项目，`pgdt.gtimg.cn`从拒绝改为直连，解决新浪无法访问。

规则地址 https://raw.githubusercontent.com/phusbot/Manual/master/Shadowrocket.Conf

[Telegram社群](https://t.me/joinchat/Eeks0Eh3DYd_ndSdcpMmyg)
