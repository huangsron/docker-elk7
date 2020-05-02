# elk udp

## Download filebeat
curl -L -O https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-7.6.2-linux-x86_64.tar.gz
tar xzvf /filebeat-7.6.2-linux-x86_64.tar.gz

## debug filebeat
./filebeat -c ./filebeat.yml  -v -e

## test filebeat
nc -w0 -u localhost 5140 <<< "testing again from my home machine"
nc -u -l 5140