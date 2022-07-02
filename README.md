# Self-hosted Azure DevOps Docker Agent

https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker?view=azure-devops

## Build

Docker build command

```bash
docker build -t azuredevopsagentlinux:latest .
```

## Usage

```python
docker run -e AZP_URL=https://dev.azure.com/{org} -e AZP_POOL={customPoolName} -e AZP_TOKEN={PAT} -e AZP_AGENT_NAME={agentName} azuredevopsagentlinux:latest
```