ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:${ELASTIC_VERSION}

# Add your logstash plugins setup here
RUN logstash-plugin install logstash-filter-dissect
RUN logstash-plugin install logstash-filter-grok
RUN logstash-plugin install logstash-filter-mutate
RUN logstash-plugin install logstash-filter-aggregate
RUN logstash-plugin install logstash-filter-date
RUN logstash-plugin install logstash-filter-csv
# Example: RUN logstash-plugin install logstash-filter-json
