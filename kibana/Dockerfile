ARG ELK_VERSION

# https://github.com/elastic/kibana-docker
FROM docker.elastic.co/kibana/kibana:${ELK_VERSION}

RUN mkdir -p /usr/share/kibana/data/wazuh/config

RUN chown -R kibana:kibana /usr/share/kibana/data

RUN /usr/share/kibana/bin/kibana-plugin install https://packages.wazuh.com/4.x/ui/kibana/wazuh_kibana-4.4.4_7.17.9-1.zip

