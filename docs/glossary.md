# Glossário com principais comandos e suas funcionalidades no _Kubernetes_

## Kubectl

Dentre as ferramentas fornecidas pelo k8s para acesso e controle dos containers temos o **kubectl** que é um runtime que se comunica diretamente com a api do k8s e atráves dele conseguimos criar/remover/alterar e manipular livremente nossos pods e containers em execução.

dentre os principais comandos estão:

- **run:** inicia um novo pod com base em uma imagem. que pode estar alocada localmente ou em um repositório de imagens como o docker hub.
  - **exemplo:** `kubectl run nginx-pod --image=nginx:latest`

- **get:** metacomando do ctl para retornar informações de consultas de diversos serviços do kubernetes, como: pods, nodes, namespaces e afins.
  - **exemplo:** `kubectl get nodes` retorna todos os nodes conectados ao cluster.

- **describe:** descreve com informações detalhadas todos os dados referentes ao objeto pedido subsequentemente.
  - **exemplo:** `kubectl describe nodes` trás a descrição detalhada de todos os nodes alocados no cluster. ou `kubectl describe pod nginx-pod` trás as informações detalhadas sobre o pod com nome 'nginx-pod'.

- **edit:** pode ser usado para efetuar edições no arquivo de configuração do pod selecionado no comando.
  - **exemplo:** `kubectl edit pod nginx-pod` abre em arquivo de texto as configurações usadas no pod 'nginx-pod' para alteração manual.

- **apply:** comando utilizado para se aplicar definições aos pods do kubernets, utilizando a flag `-f` pode ser feita a aplicação de configurações via arquivos externos que podem estar tanto em `JSON` quanto em `YAML`.
  - **exemplo:** `kubectl apply -f meu-primeiro-arquivo-definicao.yaml`

- **delete:** usada para efetuar ações de remoção dentro do k8s com o kubectl. Utilizando a tag `-f` você pode remover pods que foram criados de maneira declarativa utilizando arquivos de configuração.
  - **exemplo:** `kubectl delete pod nginx-pod`

- **annotate:**

- **rollout:**
