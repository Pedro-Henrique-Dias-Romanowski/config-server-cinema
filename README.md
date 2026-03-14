# Config Server Cinema

Este repositório contém o servidor de configuração centralizado para o sistema de gerenciamento de cinema, baseado no Spring Cloud Config Server.

## Descrição

O Config Server Cinema é responsável por fornecer configurações centralizadas para os microserviços do sistema de cinema. Ele utiliza arquivos YAML para gerenciar configurações específicas de cada serviço e ambiente (desenvolvimento e produção).

## Estrutura do Projeto

- `application.yml`: Configuração principal do servidor de configuração.
- `api-gateway/`: Configurações para o microserviço API Gateway.
  - `api-gateway.yml`: Configuração do API Gateway.
- `ms-autenticacao-cinema/`: Configurações para o microserviço de Autenticação.
  - `ms-autenticacao-cinema-dev.yml`: Configurações para ambiente de desenvolvimento.
  - `ms-autenticacao-cinema-prod.yml`: Configurações para ambiente de produção.
- `ms-gerenciamento-catalogo/`: Configurações para o microserviço de Gerenciamento de Catálogo.
  - `ms-gerenciamento-catalogo-dev.yml`: Configurações para desenvolvimento.
  - `ms-gerenciamento-catalogo-prod.yml`: Configurações para produção.
- `ms-gerenciamento-clientes/`: Configurações para o microserviço de Gerenciamento de Clientes.
  - `ms-gerenciamento-cliente-dev.yml`: Configurações para desenvolvimento.
  - `ms-gerenciamento-cliente-prod.yml`: Configurações para produção.
- `ms-gerenciamento-sessoes/`: Configurações para o microserviço de Gerenciamento de Sessões.
  - `ms-gerenciamento-sessoes-dev.yml`: Configurações para desenvolvimento.
  - `ms-gerenciamento-sessoes-prod.yml`: Configurações para produção.

## Tecnologias Utilizadas

- Spring Cloud Config Server
- YAML para configurações

## Como Usar

1. Clone o repositório.
2. Configure as propriedades necessárias no `application.yml`.
3. Execute o servidor de configuração.
4. Os microserviços podem buscar suas configurações via endpoints do Config Server.

Para mais detalhes sobre o Spring Cloud Config, consulte a [documentação oficial](https://spring.io/projects/spring-cloud-config).
