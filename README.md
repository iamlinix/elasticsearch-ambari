## Original Repo | 原地址

```
https://github.com/teamsoo/elasticsearch-ambari
```

## Compatibility | 兼容性

This service has been tested with the following:
该服务仅在以下环境中测试通过：

- Ubuntu 16.04
- Ambari 2.6
- HDP 2.6
- ElasticSearch 6.x

## Installation | 安装

```
VERSION=`hdp-select status hadoop-client | sed 's/hadoop-client - \([0-9]\.[0-9]\).*/\1/'`
sudo git clone https://github.com/iamlinix/elasticsearch-ambari.git /var/lib/ambari-server/resources/stacks/HDP/$VERSION/services/ELASTICSEARCH
```

## Required Properties | 值得注意的属性
```
zen_discovery_ping_unicast_hosts - FQDN of master and data nodes. seperated by comma eg. master.internal,data1.internal,data2.internal (集群所有节点的主机名，以逗号连接，例如： master.internal,data1.internal,data2.internal)
network_host - ethernet interface or ip address to bind. (需要绑定的网上名称或是 ip 地址)
http_port - port to bind. (需要绑定的端口)
elastic_repo - repository url for elasticsearch. (下载 elasticsearch 的源的地址)
```

## Screenshot | 截图
![Image](../master/screenshot.png?raw=true)


check my first commit for more details.
查看我的第一个 commit 了解更多的修改细节。
