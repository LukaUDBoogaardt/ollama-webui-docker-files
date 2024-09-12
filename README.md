Combine and run all docker compose files:

```bash
docker compose -f docker-compose.yaml -f docker-compose.gpu.yaml -f docker-compose.searxng.yaml up -d --remove-orphans --force-recreate
```

remove the searxng file if you don't want/need ollama to have web search access.

For amd see changes in gpu.yaml

Models I use:
- llama3.1: chat
- deepseek-coder-v2: coding using visual studio code 'continue' extension
- llava: multi modal chat