# query-chain

Sample script for executing FilterQueries against an EVM chain. Just update the rpc end point in `main.go` file to execute queries against and RPC node of choice.

By default the script queries against Rinkeby and Moonbase Alpha for a Rollup creation event.
Sample output:

```
2021/07/17 20:21:12 Rinkeby
2021/07/17 20:21:20 Querying from block: 0 to: 8953133
2021/07/17 20:21:24 rollup found!
2021/07/17 20:21:24 Moonbase
2021/07/17 20:21:25 Querying from block: 0 to: 350914
2021/07/17 20:21:35 Error filtering logs: query timeout of 10 seconds exceeded
2021/07/17 20:21:35 Moonbase
2021/07/17 20:21:35 Querying from block: 100000 to: 350915
2021/07/17 20:21:45 Error filtering logs: query timeout of 10 seconds exceeded
2021/07/17 20:21:45 Moonbase
2021/07/17 20:21:45 Querying from block: 200000 to: 350916
2021/07/17 20:21:56 Error filtering logs: query timeout of 10 seconds exceeded
2021/07/17 20:21:56 Moonbase
2021/07/17 20:21:56 Querying from block: 250000 to: 350917
2021/07/17 20:22:06 Error filtering logs: query timeout of 10 seconds exceeded
2021/07/17 20:22:06 Moonbase
2021/07/17 20:22:06 Querying from block: 300000 to: 350917
2021/07/17 20:22:12 rollup found!
2021/07/17 20:22:12 Moonbase
2021/07/17 20:22:13 Querying from block: 310000 to: 320000
2021/07/17 20:22:14 rollup found!
```

## How to use

Make sure that `golang` is installed and is in your path.
clone the rep: `git clone https://github.com/YameenMalik/query-chain.git`. Install dependencies using `go mod tidy`. Run the script using `go run .` or `go run main.go`.
