# 产品功能 


### 入侵威胁 

#### 病毒木马

病毒木马功能采用云+端的查杀机制，客户端负责采集进程信息，上报到云端控制中心进行病毒样本检测。若判断为恶意进程，支持用户隔离文件等处理，云查杀服务集成了国内外主流病毒查杀引擎，云沙箱以及威胁情报检测能力。

#### 网页木马

网页木马功能是采用本地+云端查杀机制，客户端本地通过静态检测引擎发现网页木马，同时对可疑程序上报云端判断。云端网页木马查杀引擎包括：AI查杀引擎和网页木马沙箱检测引擎。

#### 系统后门检测

rootkit是一种将自身隐藏在计算机操作系统当中的恶意软件，通过主机安全后门检测功能，提供内核级rootkit检测、应用级rootkit检测等安全能力。

#### 可疑操作

通过审计用户命令行中输入的可疑操作行为，包括：密码文件修改、 恶意文件下载、代理软件滥用、篡改系统日志、篡改ssh密钥、运行黑客工具、反弹shell、信息泄露、高危命令、破坏安全程序、明文密码登录等。

#### 敏感文件篡改

支持系统文件篡改：检测Bash、ps命令进程是否被恶意替换，隐藏的非法进程运行等，支持用户自定义文件篡改监控。


### 风险发现 


#### 合规基线

合规基线linux最佳实践分别从文件权限、服务配置、身份鉴别、入侵防范、安全审计方面，把公有云租户使用频率最高的基本配置检测呈现给用户，让租户对云主机操作系统安全配置有直观的了解，预防由于配置疏忽导致的入侵事件。

#### 账号风险

系统内置弱口令字典，根据字典规则对账号口令进行检测，通过云平台展示存在弱口令风险，提醒用户修改，避免系统账号被破解。

#### 主机漏洞

linux漏洞检测：对标CVE官方漏洞库，采用自研版本匹配引擎进行软件版本比对，对当前使用的软件版本中存在的漏洞进行告警。支持一键修复。 windows漏洞检测：同步微软官网补丁源，对高危及有影响的漏洞进行检测和提醒。支持一键修复。

#### 异常登陆

用户可以设置常用登录地区、合法登录IP、合法登录时间，当出现登录地址为非常用登录地，登录IP为非法IP，登录时间为非法时间，则产生告警记录，上报到云平台提醒用户存在异常登录风险。

#### 暴力破解

通过系统日志、网络数据包协议分析、端口等方式获取尝试暴力破解的IP，并判断其是否满足防护规则若满足规则，则进行拦截并上报云平台，同时支持用户自定义暴力破解规则，暴力破解成功。