ARG ELK_VERSION
FROM elasticsearch:${ELK_VERSION}

# 安装ik中文分词插件
RUN cd /usr/share/elasticsearch/plugins \
    && mkdir ik \
    && wget https://github.91chifun.workers.dev/https://github.com//medcl/elasticsearch-analysis-ik/releases/download/v6.4.0/elasticsearch-analysis-ik-6.4.0.zip \
    && unzip elasticsearch-analysis-ik-6.4.0.zip -d ik \
    && rm -rf elasticsearch-analysis-ik-6.4.0.zip

EXPOSE 9200 9300
