## 8.3.eID数字身份凭证认证等级3\(AAL3\)

AAL3为声明人拥有并控制了颁发给注册用户的认证器的可靠性提供了非常高的保证。AAL3的认证基于拥有密码协议的密铸。AAL3类似于AAL2,但是需要“基于硬件的、不可复制的“密码认证器来提供对抗身份冒用的能力。为了在AAL3进行认证,声明人应通过安全认证协议证明拥有和控制两种不同的认证因子。其中,经过认可的密码技术是一个必需的条件。

### 8.3.1.AAL3允诈的认证器类型

AAL3认证必须使用认证器组合中的种进行。可能的组合是:

* 多因子密码设备
* 与口令一起使用的单固子密码设备
* 与单因子密码设备一起使用的多因子OTP设备\(软件或硬件\)
* 与单因子密码软件一起使用的多因子OTP设备\(仅限硬件\)
* 与多因子密码软件一起使用的单因子OTP设备\(仅限硬件\)
* 与单因子密码软件和口令一起使用的单因子OTP设备\(仅硬件\)

### 8.3.2.AAL3要求的安全控制措施

* 声明人与认证器之间的通信必须经由安全连接的受保护通道进行,以确保认证器输出的机密性并抵抗中间人攻击。AAL3中使用的所有认证器必须具有防止身份冒用的特性,以及防止重放的特性。AAL3的所有认证和重新认证过程都必须至少从一个认证器展示认证意图。

* AAL3认证器必须对至少一个认证因子满足防止危害的特性。AAL3中的基于硬件的认证器和认证方应该可以抵制相关的旁路攻击\(例如定时和务耗分析\)。相关的旁路攻击必须由认证方进行风险评估确定。
* 当在认证过程中使用智能手机等设备时,对该设备的解锁不得被作为认证因子之一。一般来说,认证方不可能知道设备已被锁定,或者解锁过程是否符合视关认证器类型的要求。
* RP应在有限时间内依据用户所持有认证器的认证结果提供服务。如果用户长时间不活动,或者超出了认证有限期,RP需要对用户重新认证或者停止提供服务。


