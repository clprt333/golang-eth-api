Start Ganache
Connect Metamask to Ganache testnet rpc
Import private key from test account
send transaction to another account through metamask

http://localhost:8080/api/v1/eth/latest-block
Get transactions

http://localhost:8080/api/v1/eth/get-tx?hash=<tx hash>

check balance of recipient
http://localhost:8080/api/v1/eth/get-balance?address=<the-recipient-address>

curl -d '{"privKey":"f398a7b9b77d4206a1251958f477e04caa85a5d963a538bf1fff6288241cc756", "to":"0xc4fE623131dD3761F769c59457de3a1b3b41eFF8", "amount":1000000000000000000}' -H "Content-Type: application/json" -X POST http://localhost:8080/api/v1/eth/send-eth