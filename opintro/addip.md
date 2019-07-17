{{indexmenu_n>3}}

# 3、添加IP

| 机房类型 | 代理模式 | 特殊IP（可以屏蔽udp协议）     | 额外添加IP（非免费的高防IP）    |
| ---- | ---- | ------------------- | ------------------- |
| 华南高防 | 支持   | 购买保底60G以上支持         | 支持，有配额限制            |
| 华东高防 | 支持   | 杭州1 BGP高防：默认屏蔽UDP协议 | 除杭州1不支持外，其余支持，有配额限制 |
| 境外高防 | 不支持  | 不支持                 | 支持，有配额限制            |

<wrap
em>注意，华东杭州1的BGP高防默认屏蔽UDP协议，如果业务是采用UDP协议的，请使用其他线路的高防，比如华东电信高防。</wrap>

## 添加IP（代理模式）

代理模式指采用NAT代理转发的技术，由高防机房替代源站面向用户，用户访问网站先经过高防机房再由高防机房将访问发送至源站。

优势：允许添加非ucloud上的外网IP。

劣势：质量上不如直连模式更稳定，并且不能用于绑定ucloud的uhost和ulb。

![](/images/opintro/game/添加代理ip.png)

**高防线路：**建议选择和源站一致的高防线路，如果源站是BGP线路，则建议选择用户来源多的那个线路。以减少访问延迟时间。

**源站IP：**填写需要防护的源站IP，如果源站IP已经暴露，建议更换一个新IP后再填写。

**备注说明：**自定义的说明文字。

## 添加特殊IP

指能够屏蔽udp协议的IP，如果发现攻击大部分来自udp协议，采用这种高防IP，可以节省弹性防护费用。