# Distributed Digital Ecological Platform AS A Service

### download pre binary
https://github.com/tien-ds/tien-depaas/releases
### how to start
```shell script
./depaas-seed-linux-v0.1.2 init
./depaas-seed-linux-v0.1.2 run --persistent-peers tcp://520e264def1262d45910ed742865d6f835ecdc59@123.100.236.30:26656
```
#### peer list
```
tcp://520e264def1262d45910ed742865d6f835ecdc59@123.100.236.30:26656
tcp://363aaac13b215600b8f29844cd273f0c2eca175a@198.55.58.138:26656
tcp://6874612a29c7e3990cfe1aaca0e1970606ef0c44@198.55.58.204:26656

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

#### eg. invoke eth_getTransactionByHash
```
curl --location --request POST 'http://123.100.236.30:46658/eth' \
--header 'Content-Type: application/json' \
--data-raw '{
    "jsonrpc": "2.0",
    "method": "eth_getTransactionByHash",
    "params": [
        "0x80653ab611a53907853e0ed84ed4fc1928f85d40501f76d573707c0ec9dbee1d"
    ],
    "id": 1
}'
```

# how to Mortgage mining
- First you need 1.2 million DE Token
```
./depaas-seed coin approve --contract 0xe288d6eec7150D6a22FDE33F0AA2d81E06591C4d -k aa 0x01D10029c253fA02D76188b84b5846ab3D19510D 12500000
./depaas-seed dpos3 register-candidate -k aa {you publicKey} 100 3 --name node3 # register-candidate
```
> aa is you private key file

# How to sign offline ?
Reference [depaas-sdk](https://github.com/tien-ds/depaas-sdk)
