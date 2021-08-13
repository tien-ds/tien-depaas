# Distributed Digital Ecological Platform AS A Service

### download pre binary
https://github.com/tien-ds/tien-depaas/releases
### how to start
```shell script
./depaas-seed-linux-v0.1.1 init
./depaas-seed-linux-v0.1.1 run --persistent-peers tcp://520e264def1262d45910ed742865d6f835ecdc59@123.100.236.30:26656
```
#### peer list
```
tcp://520e264def1262d45910ed742865d6f835ecdc59@123.100.236.30:26656
tcp://363aaac13b215600b8f29844cd273f0c2eca175a@198.55.58.138:26656

```
### how to use 
- depass support eth rpc
```shell script
{"eth_blockNumber"},
{"eth_getBlockByNumber"},
{"eth_getBlockByHash"},
{"eth_getTransactionReceipt"},
{"eth_getTransactionByHash"},
{"eth_getCode"},
{"eth_call"},
{"eth_getLogs"},
{"eth_getBlockTransactionCountByNumber"},
{"eth_getBlockTransactionCountByHash"},
{"eth_getTransactionByBlockHashAndIndex"},
{"eth_getTransactionByBlockNumberAndIndex"},
{"eth_newBlockFilter"},
{"eth_newPendingTransactionFilter"},
{"eth_uninstallFilter"},
{"eth_getFilterChanges"},
{"eth_getFilterLogs"},
{"eth_newFilter"},
{"eth_unsubscribe"},
{"eth_getBalance"},
{"eth_estimateGas"},
{"eth_gasPrice"},
{"net_version"},
{"eth_getTransactionCount"},
{"eth_accounts"},
{"eth_getStorageAt"},
```
- support evm contract
