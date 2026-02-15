└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getblockchaininfo
{
  "chain": "main",
  "blocks": 0,
  "headers": 0,
  "bestblockhash": "0052f569e45bf266de0127bc5a6fe12dc59c3aaf9fc5dc3e1fc2ffc48d9af359",
  "bits": "2000ffff",
  "target": "00ffff0000000000000000000000000000000000000000000000000000000000",
  "difficulty": 5.960464477539062e-08,
  "time": 1771099660,
  "mediantime": 1771099660,
  "verificationprogress": 1,
  "initialblockdownload": false,
  "chainwork": "0000000000000000000000000000000000000000000000000000000000000100",
  "size_on_disk": 260,
  "pruned": false,
  "warnings": [
    "This is a pre-release test build - use at your own risk - do not use for mining or merchant applications"
  ]
}


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin createwallet "mywallet"
{
  "name": "mywallet"
}


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getnewaddress
mc1q0an5kdtxccs5570v5a2mntudtkxak5a9e8cs2c


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getnewaddress
mc1qf5w8uacezek9xg750p0c3zjummv3k2wfs7k36q


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin generatetoaddress 1 mc1qf5w8uacezek9xg750p0c3zjummv3k2wfs7k36q 10000000
[
  "00c92f94f0def460bcb79899e8c4d3e35ad4818043829c511441b31ac5eae185"
]


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getbalances
{
  "mine": {
    "trusted": 0.00000000,
    "untrusted_pending": 0.00000000,
    "immature": 50.00000000
  },
  "lastprocessedblock": {
    "hash": "00c92f94f0def460bcb79899e8c4d3e35ad4818043829c511441b31ac5eae185",
    "height": 1
  }
}


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin generatetoaddress 100 mc1qf5w8uacezek9xg750p0c3zjummv3k2wfs7k36q 10000000
[
  "005042b0f53ba71eb8beb9f7499315c8c6b735b6fd9073c6fcd3b484c4fe58a8",
  "003d7f4de6558fb887e02d9539de15d01b5c7a3819c92be1461bfff5a354eadd",
  "0029bbb0df34ee7d183942fe98765c7ab83119311b4f8a64e7869a3c51a4a93e",
  "003a209ab1dc625492eda203a683bd603de8875d85ddacc1cc464056f1b15083",
  "001bea5da513d7fb28f35548e270cd4df0dec162a373ad42029a28cb95b86c1c",
  "0079ce68395c75634c2ff705c77126d2edc57379b7360a0feef74a6499923434",
  "006096107eac82c901ec6c07bb054cdb54c3e1d62c8b554dd08f6858fff65eab",
  "00bfc1c4508ed9cf2b202aae1457e481d391dac8648a4de159f3cbf2a13aad57",
  "00cdca1293b4b4471998259e5655695b3bf45e2079822c7d7184d3f9f15723b3",
  "00f1bfdb8b175e7a1cebbd2034adaea475fda4695d113b8e2f01fde7fc48781c",
  "00a74f871cecec253606b7c73d94a8480fed222be1071ada60b79d248473858f",
  "001d96016f762aebfcc7a123d170cb867af20ce472bc13238156aa7a4b6ae525",
  "007fbadd62e84680ef68b54bb37f2d76fc4f927c35a1f06ac617d879dd34b46b",
  "0034c159ce394f2c5b68fdb58695d7565840ce06b749581db2dc8e7e53430547",
  "0065ae27b327c7e8b5da5a48599fe2843b563f7bb0bb450362cf1a7ca80a94d1",
  "0016eb28f255ef6477321f1db5c2b729240487e4eb34f2f187437c99a2cb1052",
  "00b15067038db2897fd340be38482b90056eadc2ef95e31475516111a21eddd5",
  "00d1d53ba9f2e15a8cd1dd9fd78ea12417b40b45a660886180e8da94bd2433f3",
  "00ad2f5ed87fcc7e2ca64347e06db730ee3b0b2b3f38008657fcf59957c6a4e5",
  "00e81153a77f566d6948fc13ec18179a87e33e73870a3541f886ee025dd9a883",
  "003adadeb9e1133681384b521af68e7b30cd17c3177c34c1da9c4266943dabb6",
  "0060841307733908639e634c287990e5e59c9db14f4d33282c08f4bb8bcccd37",
  "00b55e140685582ac636d04887598dd065a25639e2d761fe04b9e782d94a8a2c",
  "004644dade185d8611ddc07de51c02a5bfa7fe067f8b6dd832c851299ddff159",
  "004b84b66d8172589b3c49d82d3b6a2157c951a7a680c3e3def074c366153f69",
  "00d61009dbe8fc815158f29de3fd4f53efd590cc93e1d0518afc9cc53a7aba78",
  "0008f90650f926b5b53cb5b3a500248a74cbde2a0c4b13edc1be8d82aa609af3",
  "00e0793a05825d572ef6cbd084a896d758cba60e8d9ff0c72157e9314ef8d0a5",
  "00bcbca9f74302e4ad72660989ebdefb1d4df5ff402b70eaae2c3d502bc16fd8",
  "003a81802be90a4e982a6947b5f24cf1597133323c3355fd92fb9d10097e9e2b",
  "0008b227bb1f97f659c1c639eb0da6b819e12e27e73a127039169af5793e1418",
  "0050e1b6b5a7c6f42f46fc1a3ed0b09ab5d6da25dee0966bd20bed8994b506a2",
  "00c8b1239420d7dfeb58830e76d5d3ddc584035033e64ef710cdab7a8c87e466",
  "004f880d2cd0e8cf32e8659e032f57d688e284e8085f1fd537c536c118d4d791",
  "0077815efd96c61459ac338301403d92a4acffd461b9f74cc12621b1af29cc9c",
  "0008260bd21e0ffea32d05e8c0032fcc746cdc89585217127455339ac937912d",
  "00547dba32fd1543111b528d2ddfa3fc6c3d724e92ed3220c4d0d03ab375589a",
  "00a76f6ff5c226c2b779a29ab5fb8f87b36995741bf757eea6dd887f035875f0",
  "009ec621ad49a69827c2b5efcc88fb79fe5c89e379e5f5608ffdc830afdc18ed",
  "00dd7a5abc26d5b973d7cbf6703cb00cb73402749c3dff7dff59e149af10da28",
  "00e200ce9a48dede52086844bc2ba0fba2721c959e0792f85efb8862de486320",
  "0091b947652646416851b2bad6c18e81e9de76f40aa435928ae1e4b4959e3288",
  "00258cb9ebef41ab407b5bd7210a0aa2667d4e22c562032a8e49d8a23258b6f5",
  "0036121d385721b37637e8d0b981b09166e17f72eb19bbb9171bc57ed6f97364",
  "008000d3e8779100c7b16ca5a7aca4a00542349eb741d24b46cbd2488bd57eac",
  "000892519c9f5824d28570cec439ee15ed5c1af8af0a0a3b7a42a612d514eeaf",
  "00b1314d477fb6659c8aa3f8204e9fbecfa9f7b2e5c8ac79ac7c7448f27b0765",
  "0030429db061a13f8efb0affa83894a923362344a9c5366adc95d555af8b9be3",
  "00b5f36e232101a30043471665d3cd55fc3f521658c84b6944fc57439f040560",
  "0040c5f6946e2af15e69565bcba02e132c7967722705f73b44eb3d0d87145ccf",
  "00fd575ac63a0ec5b6da7fed76c47dce974a25ab8e85a7e1dee8009f3a5f8ab6",
  "006614f4855bdb4d8ab088f32bfc9e1be80db23eb0569b4c457bff888bc59629",
  "00f1b4220e3e2b39953138ce42695e68a88863c5a1278a442d644cd28e692423",
  "0086b14f4794cf176a68389358eefa5acae1a0d9c88ac2c18b64a3573c7da533",
  "00f33ffd1b00bce3b3571483327d820c30be77dda4a89cfdfc21185fcab96ac9",
  "00d6cfdd9b1d3364df2db84336e4e7af86a494dae3d1e0d1e6009cb0a3471123",
  "005c4f2e17417cb5a39794e3e9fceb51d07e1bd1fd39c8238dcb0a18392177ab",
  "005e2026a76d7a1b37e654a344173f0b07d06a6fe80db8a1998cba5f64537ee3",
  "00a157767289abe3fe9282f9cd595fa3d71d8e307a3c30d450b2d04cad926715",
  "0092050601df6e1beba63ef9370874192c65a01b5e10a10a5a957b330a4c549a",
  "009c855bd92f57128e926c5fd8882bd338a1b0e06cbc4e93a1991e7eac6760eb",
  "008d7f99959533a2efc5bb265c7983edd7ce8e64cc42a5a2962cb0cb534bf39b",
  "00b5d072dff8bf70d0c7228995c38e2a5191c52fb8d3bcc3ad4bff301a328f46",
  "006b1ca1114285c494b01cc35b973601bb226ee94a70fb2a33676e672f90f8dd",
  "00dc6e9d2deb6b5d8411b1352910482efde17b44bbdac702e4610cfc7dbf1d93",
  "006fe42f35b762f9e907c2d27c8635dbff005de630688f9e90a3648b11a5a2cc",
  "001c79588f6d75ca896e04392c5b8d67afa5f01b096646544e23e12ff6539426",
  "00b5a4523af911837cca45edf270044318a9ad0da3ec132f44a0f0ab8669e4f8",
  "00b601c51b934792190150c144881f08b85a47fe8c17ba5f89541c02e2391722",
  "0072a8e4df665eff043dc372b95c2399c8135629eae4fdcab58bcb535033d7e9",
  "000fb065736ea37166110e75c71436f6325c1a0b65d3af63278f8665dab91f81",
  "00c12621f2ccc9ad1d481e60a01484d867bec92953c7fa9602c24f810b09d9ef",
  "0089a64108cea7535a50bbd049481b149df803fd919bdb02b1632843b4c4ad9f",
  "00bb1b4e49dd516761b48be4c7b97e314558795333556aca81956340076e5912",
  "00b4e71e158cbf5a864e45b9b62155c3dcaddb3e6f948400b377d646253c0463",
  "00f18d987b6654172f791cbf0e92b749eca08a5eb3965d1bf5c3970998d23c07",
  "00d009f2885cea1f1d90f16b0eaeb4e97e3ae09fafc7bf5a10ecfd9a9339cd37",
  "002560df10a2053c012f10d48008b80b3786a37dd1eb36b41dc538d99cf3fe52",
  "00f5361cf43deb08b690bbd2e8418caa150eef5d5ca951b6672bc6957726866e",
  "00c97ad53b5bc6b4b16884f1f72b6735c57cfd8615ba5c38516b6b55632ccd97",
  "005fa99d0cda935fb26cf5bbcd0ce5dada94dd974588e6f63ed69c7446a434da",
  "0028a46cfc082495889026003b8889fc1a13b89bc1a548113eb45ce4262ffa57",
  "00bc0f0a833daba66793a6ee452fa49e89ba94992cf188bd66b2c7bd44e3bb1e",
  "00635180613481099b6f5e285639303b44f3126546fda99b20eee6b157f7a512",
  "0028263c402f256cb830b0842ed8bb9b605bfc3ab20768a78c9a2671b71b2a1e",
  "001828a8fe5707e2596e6526430058291dd42955a530650b87ec74e7743963a4",
  "004c342353e7c1c7978e42134add09329a95968d12cfcd5265370b61c186cb22",
  "00d95e0ae0a7ae35951efc0c9c4fca020c2454e3a1831665fe26056f4f77110c",
  "004a32d228a18555cf612cd22fcb070ddc614a7040f64b4e5e8d90d1c5aa4ce6",
  "0046b69f0fb36e8c681e8c28ec48a9c8e66801e040c455ce889a6c5c2dbc7507",
  "005a59525874ec16e2dfcc8070df147c943e650d41cf1bf47387a88e517f2aa6",
  "00dcd3df13bae7f5251ea385bca87cc337577857549d6206a9227a4f024f9b7a",
  "000b07c8ee715b3c33d532ff657375586882fc4f1ca39fd0a4b6ec730c49c5a8",
  "00083ed1fc7f1f30dde17020c27629a5bb867365ddbbdf4d5cf96844e8b366ec",
  "00d8119111ec0b23ebba9f4cec605c42b51edeab2bc0270747f1eecde3b8d40a",
  "0038e1b16260172a735e2ca177ed6ccc3580a0d758fcecd424933b3d90e7f599",
  "0011f6eeec286aa0a3af1298277b89397ece89b57ecbd4520206207c38661d71",
  "00bc05da290312bd6f0ba081cee6c810359b9175b41282404078230818285742",
  "00d6cb62fd039364307083f3df7ea92a3a143600f0a267a7ef07cc0e3d01b341",
  "00183253f58c4396e9e100c39350fa9fbdfe3b08a4a9ad28f8435abd1e3c62e2"
]


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getbalances                                                              
{
  "mine": {
    "trusted": 50.00000000,
    "untrusted_pending": 0.00000000,
    "immature": 5000.00000000
  },
  "lastprocessedblock": {
    "hash": "00183253f58c4396e9e100c39350fa9fbdfe3b08a4a9ad28f8435abd1e3c62e2",
    "height": 101
  }
}


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getbalance                                                               
50.00000000


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getbalances
{
  "mine": {
    "trusted": 50.00000000,
    "untrusted_pending": 0.00000000,
    "immature": 5000.00000000
  },
  "lastprocessedblock": {
    "hash": "00183253f58c4396e9e100c39350fa9fbdfe3b08a4a9ad28f8435abd1e3c62e2",
    "height": 101
  }
}


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin generatetoaddress 1 mc1qf5w8uacezek9xg750p0c3zjummv3k2wfs7k36q 10000000 
[
  "00c34f26b0c140fa4c62ba20a4f35f523672e29d165fef29e2476df4d3228483"
]


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getbalances                                                            
{
  "mine": {
    "trusted": 100.00000000,
    "untrusted_pending": 0.00000000,
    "immature": 5000.00000000
  },
  "lastprocessedblock": {
    "hash": "00c34f26b0c140fa4c62ba20a4f35f523672e29d165fef29e2476df4d3228483",
    "height": 102
  }
}


┌──(kibato㉿Champollion)-[~/Desktop/Thesis/bitcoin]
└─$ ./build/bin/bitcoin-cli -datadir=/tmp/mycoin getbalance                                                             
100.00000000
