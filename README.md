# What is holer
Holer exposes local servers behind NATs and firewalls to the public internet over secure tunnels. <br/>
Support forwarding message based on TCP protocol.<br/><br/>
Holer是一个将局域网服务器代理到公网的内网穿透工具，支持转发基于TCP协议的报文。
![Demo](https://github.com/Wisdom-Projects/holer/blob/master/Image/demo.png)
# How it works
#### 1. Download software package [*`holer-client.zip`*](https://github.com/Wisdom-Projects/holer/blob/master/Binary);
下载软件包[`holer-client.zip`](https://github.com/Wisdom-Projects/holer/blob/master/Binary)；

#### 2. Install `Java 1.7` or higher version;
使用前请先安装`Java 1.7`或者更高版本；

#### 3. Unzip `holer-client.zip`, modify configuration file
解压`holer-client.zip`，修改配置文件<br/>
`holer-client/conf/holer.conf`<br/><br/>
Only need to set `HOLER_ACCESS_KEY`:<br/>
只需设置`HOLER_ACCESS_KEY`：

`HOLER_ACCESS_KEY=HOLER_CLIENT-2F8D8B78B3C2A0AE`<br/>
     
#### 4. Start holer
启动Holer服务<br/>
`cd holer-client/bin`<br/><br/>
**Windows**:<br/>
Run command `startup.bat` or double click `startup.bat`<br/><br/>
**Linux**:<br/>
Run command `sh startup.sh`
     
#### 5. Internet and local address mapping
公网和内网的地址映射关系

Holer Access Key             |Internet Address   | Local Address
-----------------------------|-------------------|---------------
HOLER_CLIENT-2F8D8B78B3C2A0AE|holer.org:65530|127.0.0.1:8080
HOLER_CLIENT-3C07CDFD1BF99BF2|holer.org:65531|127.0.0.1:8088
HOLER_CLIENT-2A623FCB6E2A7D1D|holer.org:65532|127.0.0.1:80
HOLER_CLIENT-AF3E6391525F70E4|holer.org:65533|127.0.0.1:3389
HOLER_CLIENT-822404317F9D8ADD|holer.org:65534|127.0.0.1:22

#### 6. Demo
使用示例<br/><br/>
If your tomcat program local URL: <br/>
如果您本地的tomcat服务地址：<br/>
`http://127.0.0.1:8088`<br/>

Exposes to the public internet URL: <br/>
代理到公网上的服务地址为：<br/>
`http://holer.org:65531`<br/>

Only need to modify configuration file to set `HOLER_ACCESS_KEY`: <br/>
只需要在配置文件里修改`HOLER_ACCESS_KEY`即可：<br/>
`holer-client/conf/holer.conf`<br/>
`HOLER_ACCESS_KEY=HOLER_CLIENT-3C07CDFD1BF99BF2`<br/>

Restart holer, then you can visit your web application through URL `http://holer.org:65531`<br/>
重启Holer，然后就可以通过URL `http://holer.org:65531`来访问您的Web应用。<br/>

Please refer to [**the blogs**](http://wdom.net:9000/tag/Holer) for more demos and help.<br/>
请参考[**博客文章**](http://wdom.net:9000/tag/Holer)获得更多的使用示例和帮助。<br/>

#### 7. Other Holer Softwares
其他的Holer软件<br/><br/>
These Holer softwares ([source code](https://github.com/Wisdom-Projects/holer/tree/master/SourceCode/Go)，[package](https://github.com/Wisdom-Projects/holer/tree/master/Binary/Go)) are implemented by GO, and support many different OS and hardware architectures. <br/>
这些Holer软件（[源代码](https://github.com/Wisdom-Projects/holer/tree/master/SourceCode/Go)，[软件包](https://github.com/Wisdom-Projects/holer/tree/master/Binary/Go)）是由GO语言实现，支持多种操作系统和硬件架构。<br/><br/>
Take `Windows & Linux x86-64bit` as an example, execute the following commands:<br/>
这里以`Windows & Linux x86-64bit` 为例，执行如下命令：<br/><br/>
**Windows**:<br/>
`holer-windows-amd64.exe -k HOLER_CLIENT-2F8D8B78B3C2A0AE`<br/><br/>
**Linux**:<br/>
`./holer-linux-amd64 -k HOLER_CLIENT-2F8D8B78B3C2A0AE`<br/>

# Support
All of the above holer access keys and ports have been shared to public. In order to enable users to get more shared holer services, every user can use each holer access key to get holer service.<br/><br/>
If you want to have **exclusive holer service**, please contact by QQ for application. For more details about holer service, please visit [**Wisdom**](http://www.wdom.net).<br/><br/>
以上的全部Holer Access Key和端口都已公开共享，为了让用户获得到更多的共享的Holer服务，每个用户可以使用每一个Holer Access Key获取到Holer服务。<br/><br/>
如果您需要**独享的Holer服务**，请QQ联系开通。更多的Holer服务详情，请访问[**Wisdom**](http://www.wdom.net)。<br/>
_**QQ**    : 2353941272_<br/>

# Donate
如果 **Holer** 工具对您帮助很大，并且您很愿意支持工具的后续开发和维护，您可以扫下方二维码随意打赏，就当是请我喝杯茶或是咖啡，将不胜感激。 **♥ 谢谢 ♥**

If the **Holer** helps you a lot, and you would like to support this tool's further development and the continuous maintenance of this tool. You can sweep the following QR code free to donate me, which asked me to have a cup of tea or coffee. Your donation is highly appreciated. **♥ Thank you ♥** <br/>

**♥ Donate ♥ by Alipay, WeChat Pay**.

![Donate by pay](https://github.com/Wisdom-Projects/rest-client/blob/master/images/donate_pay.png)
