The goal of this project is to build a basic SIEM using docker compose using Elastic Stack and Nginx web proxy

The first step would be installing Elasticsearch with Docker using the following script below to pull the image:

docker pull docker.elastic.co/elasticsearch/elasticsearch:7.0.1@


The next step would be to running the script below in your terminal/command line:

docker run -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.0.1