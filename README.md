# kubernetes-mcp-vscode-githubcopilot
Configurações para uso do MCP Server do Kubernetes (npm) com Visual Studio Code + GitHub Copilot. 

MCP Server para Kubernetes "oficial": https://github.com/containers/kubernetes-mcp-server

Arquivo **mcp.json** (diretório **.vscode**):

```json
{
	"servers": {
		"mcp-kubernetes": {
			"type": "stdio",
			"command": "npx",
			"args": [
				"-y", "kubernetes-mcp-server@latest"
			]
		}
	}
}
```

Um exemplo de teste com este MCP Server:

![Consultando logs de um CronJob 1](img/k8s-mcp-01.png)

![Consultando logs de um CronJob 2](img/k8s-mcp-02.png)

![Consultando logs de um CronJob 3](img/k8s-mcp-03.png)