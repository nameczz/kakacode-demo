# Install Milvus

Download docker-compose.yml:

`wget https://github.com/milvus-io/milvus/releases/download/v2.0.0-rc7/milvus-standalone-docker-compose.yml -O docker-compose.yml`{{execute}}

Download vectors.csv, we will use it when import datas:

`wget https://raw.githubusercontent.com/milvus-io/milvus_cli/main/examples/import_csv/vectors.csv`{{execute}}

Download search.csv, we will use it when do vector search:

`wget https://raw.githubusercontent.com/milvus-io/milvus_cli/main/examples/import_csv/search_vectors.csv`{{execute}}

Run milvus in the backend:

`docker-compose up -d`{{execute}}
