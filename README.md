# 使用快照

## 解压下载的文件
```
tar -zxvf xxxx.tar.gz
```

## 修改config.ini文件，加载producer_api_plugin
```config.ini
plugin = eosio::producer_plugin
plugin = eosio::producer_api_plugin
```

## 从快照文件中启动新节点
```bash
./nodeos --config-dir=./testconfig/config --data-dir=./emptydata --snapshot=./snapshots/snapshot-00026ec1a4bfebb0c3a32e81c54856798ebc6c564d853321e0cc6aa4d5da8259.bin
```

**使用快照的时候data-dir指向一个空文件夹**
