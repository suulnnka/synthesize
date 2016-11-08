只支持 Ubuntu 14.04 LTS. 

### install

```
$ cd synthesize
$ sudo ./install

# 出错就重跑
# localhost:8180

# 配置spark
# vim $SPARK_HOME/conf/metrics.properties

# 安装 grafana
$ wget https://grafanarel.s3.amazonaws.com/builds/grafana_3.1.1-1470047149_amd64.deb
$ sudo apt-get install -y adduser libfontconfig
$ sudo dpkg -i grafana_3.1.1-1470047149_amd64.deb

# localhost:3000

# 启动
$ sudo service carbon-cache start
$ sudo service memcached start
$ sudo service collectd start
$ sudo service apache2 start
$ sudo service statsite start
$ sudo service grafana-server start

# 启动后配置grafana
```
