Open AI WEB docker compose config

## Up and running

1. Up services:

```sh
docker compose up -d
```

2. Check `localhost:3000` for Open WEB UI. And `localhost:3001` for Ollama API.

## How to pull model

1. Find model you want on [ollama site](https://ollama.com/library)
2. Pull new model:

```sh
docker exec ainekko-ollama-1 ollama pull <model_name>
```

3. After model has been pulled you can select it in Open WEB UI

## Ollama configs

On first startup ollama directory with access keys and model files is mounted to `./apps/ollama/.ollama` directory. So any time you can check your access keys.