# llm-zoomcamp-homework1

This repository contains the code and materials for the first homework assignment of the LLM ZoomCamp.

To work on this homework assignment, it is recommended to either use GitHub Codespaces or set up a local development environment.

If you prefer using GitHub Codespaces, you can simply click on the "Code" button above the file list, then select "Open with Codespaces" to launch a fully configured development environment in your browser. This will allow you to edit the code and materials directly in the cloud without any local setup.

Before running the Jupyter notebook, we need to use the following Docker command:

```bash
docker run -it \
    --rm \
    --name elasticsearch \
    -p 9200:9200 \
    -p 9300:9300 \
    -e "discovery.type=single-node" \
    -e "xpack.security.enabled=false" \
    docker.elastic.co/elasticsearch/elasticsearch:8.4.3
```

This Docker container is an instance of Elasticsearch version 8.4.3. It is used for running Elasticsearch, a distributed search and analytics engine, with specific configurations.

To run the code that makes calls to the OPENAI API, you will need to obtain an API key. 


