# Task Management

Desafio técnico para o processo seletivo da Artefact: desenvolvimento de uma aplicação simples de gerenciamento de tarefas com Next.js 15, React e tRPC.

O foco é construir uma solução simples e funcional, com validação de dados, tratamento de erros e feedback para o usuário.

## Contexto

A aplicação deverá permitir criar, listar, editar e excluir tarefas.
O backend será exposto via tRPC e manterá os dados em memória, sem necessidade de banco de dados. Os dados não terão persistência garantida entre reinicializações da aplicação.

## Tecnologias exigidas

- Next.js 15
- React
- tRPC

## Requisitos

### Modelagem das tarefas

Cada tarefa deverá conter:

| Campo | Tipo | Descrição |
| --- | --- | --- |
| `id` | Identificador único | Gerado automaticamente |
| `titulo` | String | Obrigatório |
| `descricao` | String | Opcional |
| `dataCriacao` | Timestamp | Data e hora da criação |

### Backend

- [ ] Manter as tarefas em memória.
- [ ] Implementar criação de tarefas via tRPC.
- [ ] Implementar listagem de tarefas via tRPC.
- [ ] Implementar atualização de tarefas via tRPC.
- [ ] Implementar exclusão de tarefas via tRPC.
- [ ] Impedir a criação de tarefas sem título.
- [ ] Retornar erros claros para operações inválidas, como editar uma tarefa inexistente.

### Frontend

#### Listagem de tarefas

- [ ] Pré-carregar a lista utilizando Server-Side Rendering (SSR).
- [ ] Exibir as tarefas em um layout simples.
- [ ] Permitir a exclusão diretamente na listagem.
- [ ] Exibir feedback de sucesso ou erro ao excluir uma tarefa.

#### Criação e edição

- [ ] Criar formulário para adicionar tarefas.
- [ ] Permitir a edição de tarefas existentes.
- [ ] Utilizar componentes funcionais e hooks para gerenciar o estado do formulário.
- [ ] Validar os dados antes do envio, impedindo o envio de título vazio.

#### Experiência do usuário

- [ ] Exibir estados de carregamento.
- [ ] Informar quando uma operação for concluída com sucesso.
- [ ] Exibir mensagens para erros do frontend e do backend.

## Bônus

- [ ] Implementar infinite scroll para carregar tarefas incrementalmente.
- [ ] Documentar as principais decisões de implementação.
- [ ] Adicionar comentários quando necessários para esclarecer decisões não óbvias.

## Como executar

[todo]

## Decisões técnicas

[todo]

## Dados e segurança

Todos os dados utilizados deverão ser fictícios. Não devem ser incluídos dados pessoais, senhas, tokens ou outras informações sensíveis no repositório.
