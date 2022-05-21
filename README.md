# Bug bounty for coinbase

- Set up the react project like the docs https://docs.cloud.coinbase.com/wallet-sdk/docs/web3-react until the step `access connection, account, network information`
- Dependencies in the package.json file
- https://docs.cloud.coinbase.com/wallet-sdk/docs/web3-react#access-connection-account-network-information

## Bug 1: Syntax error
- The docs includes a syntax error: a string is wrapped inside a "{}"

```bash
SyntaxError: /test-docs/src/App.js: Unexpected token, expected "}" (36:23)
  34 |       <button onClick={deactivate}>Disconnect</button>
  35 |
> 36 |       <div>{Connection Status: ${active}}</div>
     |                        ^
  37 |       <div>Account: ${account}</div>
  38 |       <div>Network ID: ${chainId}</div>
  39 |     </div>
```
