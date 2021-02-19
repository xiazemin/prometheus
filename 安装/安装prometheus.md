https://prometheus.io/download/


tar xvfz prometheus-*.tar.gz
cd prometheus-*

cd /Users/xiazemin/software/prometheus-2.24.1.darwin-amd64

./prometheus

http://127.0.0.1:9090/graph?g0.expr=&g0.tab=1&g0.sta


在prometheus文件目录中有一个prometheus.yml文件，使用的是是整个Prometheus运行的主配置文件，其中默认配置包含了大多标准配置及自控配置：



参考：
https://my.oschina.net/u/3293263/blog/1627306
https://www.lijiaocn.com/soft/prometheus/
https://zhuanlan.zhihu.com/p/63213282

https://blog.51cto.com/youerning/2050543