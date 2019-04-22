ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
RUN logstash-plugin install logstash-input-jdbc
RUN logstash-plugin install logstash-output-elasticsearch
ADD mysql-connector-java-5.1.47-bin.jar /usr/share/logstash/mysql-connector-java-5.1.47-bin.jar
