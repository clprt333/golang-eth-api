Start Ganache
Connect Metamask to Ganache testnet rpc
Import private key from test account
send transaction to another account through metamask

http://localhost:8080/api/v1/eth/latest-block
Get transactions

http://localhost:8080/api/v1/eth/get-tx?hash=<tx hash>

check balance of recipient
http://localhost:8080/api/v1/eth/get-balance?address=<the-recipient-address>

curl -d '{"privKey":"TESTNET PRIV KEY HERE", "to":"TESTNET ADDR HERE", "amount":1000000000000000000}' -H "Content-Type: application/json" -X POST http://localhost:8080/api/v1/eth/send-eth
