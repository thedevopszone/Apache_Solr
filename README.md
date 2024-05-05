# Apache Solr


## Ubuntu 22.04

```
apt update
apt upgrade

sudo apt install default-jdk

wget https://archive.apache.org/dist/lucene/solr/8.11.0/solr-8.11.0.tgz
tar xzf solr-8.11.0.tgz solr-8.11.0/bin/install_solr_service.sh --strip-components=2

bash ./install_solr_service.sh solr-8.11.0.tgz

service solr start
service solr status

ufw allow 8983/tcp
ufw enable
```
