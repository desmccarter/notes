## Create contract using JSON file

```json
var contractAddress = "0xc727b9e7b84dd34ca55f7c303df76d5f589cf2bf";
var fs = require("fs");
var jsonFile = "[[PATH TO JSON FILE]]";
var parsed = JSON.parse(fs.readFileSync(jsonFile));
var abi = parsed.abi;
var graffContract = web3.eth.contract(abi,contractAddress);
```
