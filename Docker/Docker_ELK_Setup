#Docker details to start ELK Stack 

#Pull 7.6.1 version of Elk
sudo docker pull sebp/elk:761

#Run the full stack on docker 
sudo docker run --ulimit nofile=65535:65535 -p 5601:5601 -p 9200:9200 -p 5044:5044 -it --name elk sebp/elk:761

#Login to docker container
docker exec -it /elk /bin/bash

#Update logstash input and output files  "03-s3-input.conf" and "30-output.conf" as example in the document. Upload these files with your access id, token id and variable details in /etc/logstash/conf.d/

#Add patterns file under /etc/logstash/patterns directory

#Restart your logstash from docker container
/etc/init.d/logstash restart



