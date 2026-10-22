# NexDesk 🚀

**Plataforma de Help Desk inteligente com processamento assíncrono e Inteligência Artificial.**

O NexDesk é um projeto de Help Desk desenvolvido com o objetivo de explorar conceitos de arquitetura backend, mensageria e integração com Inteligência Artificial. A plataforma busca otimizar o gerenciamento de chamados de suporte, automatizar tarefas e tornar o atendimento mais eficiente.

O projeto está em desenvolvimento e faz parte do meu portfólio, com foco no aprofundamento de conhecimentos em Java Backend e boas práticas de desenvolvimento de software.

## 🎯 Objetivo do projeto

Desenvolver uma API REST capaz de gerenciar chamados de suporte técnico, utilizando processamento assíncrono para executar tarefas em segundo plano e Inteligência Artificial para auxiliar na análise e classificação dos chamados.

## ✨ Funcionalidades planejadas

 Cadastro e autenticação de usuários.
 Gerenciamento de chamados de suporte (criação, consulta, atualização e encerramento).
 Controle de status e prioridade dos chamados.
 Comunicação assíncrona utilizando RabbitMQ.
 Processamento de eventos por consumidores independentes.
 Integração com Inteligência Artificial para classificação de chamados e sugestão de respostas.
 Registro de eventos e histórico de alterações.
 Documentação da API com Swagger/OpenAPI.
 Containerização da aplicação com Docker.
 Deploy em ambiente de nuvem.

## 🛠️ Tecnologias

As tecnologias previstas para o desenvolvimento são:

| Tecnologia                  | Finalidade                             |
| --------------------------- | -------------------------------------- |
| Java                        | Linguagem principal                    |
| Spring Boot                 | Desenvolvimento da aplicação backend   |
| Spring Data JPA / Hibernate | Persistência e mapeamento de dados     |
| Spring Security             | Autenticação e autorização             |
| PostgreSQL                  | Banco de dados relacional              |
| RabbitMQ                    | Mensageria e processamento assíncrono  |
| Docker                      | Containerização da aplicação           |
| Swagger / OpenAPI           | Documentação dos endpoints             |
| Inteligência Artificial     | Classificação e auxílio no atendimento |
| AWS                         | Hospedagem e infraestrutura em nuvem   |

*As tecnologias e funcionalidades poderão ser ajustadas durante a evolução do projeto.*

## 🏗️ Arquitetura proposta

O NexDesk pretende utilizar uma arquitetura orientada a eventos para desacoplar o gerenciamento dos chamados das tarefas executadas em segundo plano.

Fluxo simplificado:

1. O usuário cria um chamado por meio da API REST.
2. A aplicação valida os dados e registra o chamado no PostgreSQL.
3. Um evento é publicado em uma fila do RabbitMQ.
4. Um consumidor processa o evento de forma assíncrona.
5. O processamento pode envolver classificação por IA, geração de sugestões ou outras tarefas automatizadas.
6. O resultado é registrado e disponibilizado para consulta.

Essa abordagem permite estudar comunicação assíncrona, desacoplamento entre componentes, tratamento de falhas e processamento de mensagens.

## 🧠 Aplicação de Inteligência Artificial

A IA será utilizada como recurso de apoio ao atendimento, e não como substituta obrigatória da equipe de suporte.

Entre as possibilidades estão:

- Classificação automática de chamados por categoria.
- Identificação de prioridades sugeridas.
- Geração de respostas iniciais para os atendentes.
- Resumo do problema relatado pelo usuário.

As sugestões geradas deverão ser tratadas como recomendações, permitindo revisão humana quando necessário.

## 🚧 Status do projeto

**Em desenvolvimento.**

O desenvolvimento será realizado de forma incremental, priorizando inicialmente a estrutura da API, o gerenciamento de chamados e a integração com RabbitMQ. Os recursos de Inteligência Artificial e a implantação em nuvem serão incorporados conforme a evolução do projeto.

## 📚 Objetivos de aprendizado

Com este projeto, pretendo aprofundar meus conhecimentos em:

- Desenvolvimento de APIs REST com Java e Spring Boot.
- Modelagem de entidades e persistência com PostgreSQL.
- Autenticação e autorização com Spring Security.
- Mensageria com RabbitMQ.
- Processamento assíncrono e arquitetura orientada a eventos.
- Integração de serviços com Inteligência Artificial.
- Containerização e deploy em nuvem.
- Boas práticas de organização, manutenção e documentação de código.

## 👨‍💻 Autor

**Kayke Simão**

- GitHub: [@KaykeS8](https://github.com/KaykeS8)
