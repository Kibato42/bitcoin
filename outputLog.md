└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getblockchaininfo
{
  "chain": "main",
  "blocks": 0,
  "headers": 0,
  "bestblockhash": "00000000e822dce42a5b9fb2fd9609c65140cb249f8d954bdd8701503f59d114",
  "bits": "1d00ffff",
  "target": "00000000ffff0000000000000000000000000000000000000000000000000000",
  "difficulty": 1,
  "time": 1771099660,
  "mediantime": 1771099660,
  "verificationprogress": 1,
  "initialblockdownload": false,
  "chainwork": "0000000000000000000000000000000000000000000000000000000100010001",
  "size_on_disk": 260,
  "pruned": false,
  "warnings": [
    "This is a pre-release test build - use at your own risk - do not use for mining or merchant applications"
  ]
}


└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin createwallet "mywallet"
{
  "name": "mywallet"
}


└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getnewaddress
mc1qv7dfcchaa7qn5x6nuewh7k8uvav00f6skx0855


└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getnewaddress
mc1qjdftxv67nuyk3c8clvu8d5prtgl5jxwsms639w (minage)


└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin generatetoaddress 1 mc1qjdftxv67nuyk3c8clvu8d5prtgl5jxwsms639w 10000000
[
  "000000009383cb675896029795af65b6b714536fdb95b7abff3ebc61330f463b"
]


└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getblockchaininfo
{
  "chain": "main",
  "blocks": 1,
  "headers": 1,
  "bestblockhash": "000000009383cb675896029795af65b6b714536fdb95b7abff3ebc61330f463b",
  "bits": "1d00ffff",
  "target": "00000000ffff0000000000000000000000000000000000000000000000000000",
  "difficulty": 1,
  "time": 1771155924,
  "mediantime": 1771155924,
  "verificationprogress": 1,
  "initialblockdownload": false,
  "chainwork": "0000000000000000000000000000000000000000000000000000000200020002",
  "size_on_disk": 557,
  "pruned": false,
  "warnings": [
    "This is a pre-release test build - use at your own risk - do not use for mining or merchant applications"
  ]
}


└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getbalance
0.00000000


└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getblock 000000009383cb675896029795af65b6b714536fdb95b7abff3ebc61330f463b
{
  "hash": "000000009383cb675896029795af65b6b714536fdb95b7abff3ebc61330f463b",
  "confirmations": 1,
  "height": 1,
  "version": 536870912,
  "versionHex": "20000000",
  "merkleroot": "8ed8e67fa6d5bda7c487ae47e63a9374dc38363ba8f95b912bcdf4e54649f0dc",
  "time": 1771155924,
  "mediantime": 1771155924,
  "nonce": 1043595,
  "bits": "1d00ffff",
  "target": "00000000ffff0000000000000000000000000000000000000000000000000000",
  "difficulty": 1,
  "chainwork": "0000000000000000000000000000000000000000000000000000000200020002",
  "nTx": 1,
  "previousblockhash": "00000000e822dce42a5b9fb2fd9609c65140cb249f8d954bdd8701503f59d114",
  "strippedsize": 212,
  "size": 248,
  "weight": 884,
  "tx": [
    "8ed8e67fa6d5bda7c487ae47e63a9374dc38363ba8f95b912bcdf4e54649f0dc"
  ]
}


└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getbalances
{
  "mine": {
    "trusted": 0.00000000,
    "untrusted_pending": 0.00000000,
    "immature": 50.00000000
  },
  "lastprocessedblock": {
    "hash": "000000009383cb675896029795af65b6b714536fdb95b7abff3ebc61330f463b",
    "height": 1
  }
}