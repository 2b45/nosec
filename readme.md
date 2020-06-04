# 无界安全 (让天下没有难做的安全)


## 思路
> 参考 [mars](https://github.com/TideSec/Mars) / [celerystalk](https://github.com/sethsec/celerystalk) / [Langsrc](https://github.com/actanble/LangSrcCurise)

步骤如下

- 1, 通过域名爆破找到子域名的资产、通过ip查找服务
- 2, 扫描出具体的协议、服务版本等。`masscan + nmap `
- 3, 针对对应的协议/服务调用对应的脚本
- 4, 针对服务或者协议调用Poc检测
- 5, 没有了。到这里就结束了。后渗透暂不开发。

## 技术栈
- Python3.6 / django / celery / apscheduler 
- mysql 5.7 / elasticsearch 7.3 / kafka 2.4 / redis 4.0.9 
- docker-ce 19.03 主要打包脚本服务、工具服务等。
