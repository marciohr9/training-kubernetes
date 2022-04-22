# Glossário com principais comandos e suas funcionalidades no _Kubernetes_

## Kubectl

Dentre as ferramentas fornecidas pelo k8s para acesso e controle dos containers temos o __kubectl__ que é um runtime que se comunica diretamente com a api do k8s e atráves dele conseguimos criar/remover/alterar e manipular livremente nossos pods e containers em execução.

dentre os principais comandos estão:

- __run__: inicia um novo pod com base em uma imagem. que pode estar alocada localmente ou em um repositório de imagens como o docker hub.
  - __exemplo:__ `kubectl run nginx-pod --image=nginx:latest`
