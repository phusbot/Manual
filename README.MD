CloudGate Manual
==========

基于[CloudGate](https://github.com/BurpSuite/Manual)修改的规则，本人目前使用Shadowrocket，所以只修改了Shadowrocket规则。

修改目的：因为我的服务器屏蔽了国内的服务（[项目地址](https://github.com/phusbot/ss-iptables-blockade)），使用原规则时发现新浪微博用不了，因原规则把新浪的域名也添加到代理规则里。

修改处：将`sina.com`和`baidu.jp`从代理修改为直连模式。新增`360.cn`为直连。合并`umeng.com`规则并屏蔽后缀。删除`Rewrite=>Old_Rule_WebSite_Jump`项目。`pgdt.gtimg.cn`从拒绝改为直连，解决新浪微博无法访问。删除重复的规则`DOMAIN-SUFFIX,feih.com.cn,REJECT`。新增`gostats`（网站统计）系列网址为屏蔽。
精简版基于上述修改的地方再精简代理规则，删掉多余（万年都用不上）的代理规则600余条，保留常用代理规则。

规则未来解决的问题：修复无法访问知乎的问题。删除免费空间提供的网址。删除无效的网址。

规则地址 https://raw.githubusercontent.com/phusbot/Manual/master/Shadowrocket.Conf

代理规则精简版地址 https://raw.githubusercontent.com/phusbot/Manual/master/Shadowrocket-lite.Conf

[Telegram社群](https://t.me/joinchat/Eeks0Eh3DYd_ndSdcpMmyg)
