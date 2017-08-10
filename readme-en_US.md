# OpenRASP

### Introduction

Unlike perimeter control solutions like WAF, OpenRASP directly integrates its protection engine into the application server by instrumentation. It can monitor various events including database queries, file operations and network requests etc.


### Quick Start

See detailed installation instructions [here](http://rasp.baidu.com/doc/install/main.html)

We also provided a few test cases that are corresponding to OWASP TOP 10 attacks, [download here](http://rasp.baidu.com/doc/install/testcase.html)

### FAQ

##### 1. List of supported web application servers

Only Java based web application servers are supported for now. The support of other web application servers will also be soon included in the coming releases.


* Tomcat 6-8
* JBoss 4.X
* WebLogic 11/12

##### 2. Performance impact on application servers

We ran multiple intense and long-lasting stress tests prior to release. Even in the worst-case scenario (where the hook point got continuously triggered) the server’s performance was only reduced by 5%

##### 3. Integration with existing SIEM or SOC

OpenRASP logs alarms in JSON format, which can be easily picked up by LogStash, rsyslog or Flume.

##### 4. How to develop a new plugin?

A plugin receives a callback when an event occurs. It then determines if the current behavior is malicious and blocks the associated request if necessary.

Detailed plugin development instructions can be found [here](http://rasp.baidu.com/doc/dev/main.html)

### Contact

Technical support (Simplified Chinese):

* [Baidu Security Forum](http://anquan.baidu.com/bbs)
* [RASP QQ group #1: 259318664](http://shang.qq.com/wpa/qunwpa?idkey=5016bac5431b23316a79efdcd2c4dadd6ef8b99b231e4ed10f1e265573a66e1c)

Business inquires, comments, concenrs and opinions:

* General email: `fuxi-pm # baidu.com`








