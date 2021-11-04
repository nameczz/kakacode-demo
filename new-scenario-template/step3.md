# How to use milvus

## Create collection

`create collection -c car -f id:INT64:primary_field -f vector:FLOAT_VECTOR:128 -f color:INT64:color -f brand:INT64:brand -p id -a -d 'car_collection'`{{execute}}

## Create partition

`create partition -c car -p new_partition -d test_add_partition`{{execute}}

## Import datas

`import -c car './vectors.csv'`{{execute}}

## Load collections

`load -c car`{{execute}}

## Describe collection infos

`describe collection -c car`{{execute}}

## Do vector seach

`search`{{execute}}
collection name :`car`{{execute}}
import search csv: `./search_vectors.csv`{{execute}}
vector field name: `vector`{{execute}}
round_decimal: `-1`{{execute}}
topk: `10`{{execute}}
filter: `[]`{{execute}}
partition: `_default`{{execute}}
timeout : `[]`{{execute}}
