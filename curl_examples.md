## Creating index "products"

```bash
curl -X PUT http://0.0.0.0:9200/products
```

## Index a product using a string (uuid) as _id

```bash
curl -X PUT -H "Content-Type: application/json" -d @data_put.json http://0.0.0.0:9200/products/_doc/e0d97f98-26f2-4c62-9992-5cd5a89e9cf9
```

## bulk request

```bash
curl -s -H "Content-Type: application/json" -X POST http://0.0.0.0:9200/_bulk --data-binary @data_bulk; echo
```

## Very simple search

```bash
curl http://0.0.0.0:9200/products/_search?pretty; echo
```





