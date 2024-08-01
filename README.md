# LemoGPT

The goal of LemoGPT was to create a simple (variant of a) RAG (Retrieval-Augmented Generation) agent that can summarise the political and social developments in German history based on the information of [Deutsches Historisches Museum](https://www.dhm.de/lemo/) given a specific user question. The reason for the creation of this agent is to help my father write his bibliography.

### API Key
To use LemoGPT one has to add .env file with a valid OpenAI API Key like this:

```python
OPENAI_API_KEY=<key>
```

### Local results
When running LemoGPT all answers are stored in the ```answers``` folder with a timestamp.

### Run as Docker container
Use following commands to build and use the docker container

```
docker build -t lemo_gpt
docker run --rm -p 8501:8501 lemo_gpt
```
Then go to your browser and visit ```http://localhost:8501/```
