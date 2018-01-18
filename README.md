#Demo for developing lambda APIs on aws with sam local

$ sam local start-api 
$ sam local start-api -n env.json

Formato de env.json

```
{
    "Establecimientos": {
        "MONGODB_ATLAS_CLUSTER_URI":"mongodb://user:password@cluster0-shard-00-00-...&authSource=admin"
    }
    
}
```
##
PACKAGE THE FILE
```
$ sam package --template-file template.yaml --s3-bucket elm_sambucket --output-template-file package.yaml
```
