# Sample invoke for pushing QR detail on-chain

``` sh
curl -X POST 'http://localhost:3000/invoke' \
  -H 'Content-Type: application/x-www-form-urlencoded' \
  --data 'channelid=mychannel' \
  --data 'chaincodeid=fish' \
  --data 'function=CreateAsset' \
  --data-urlencode 'args@asset.json'
```

# Sample query for getting QR details

``` sh
curl 'http://localhost:3000/query?channelid=mychannel&chaincodeid=fish&function=ReadAsset&args=1' 
```
