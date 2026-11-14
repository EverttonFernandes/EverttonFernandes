<div align="center">

<img src="assets/hero.svg" alt="Everton Fernandes: Engenheiro de Software e Professor. Ilustração autoral conectando APIs, agentes, ferramentas, LLM, RAG e dados." width="100%" />

**Engenharia de Software como fundamento. IA como novo campo de construção.**

[Projetos](#projetos-com-código) · [Engenharia](#como-eu-penso-engenharia) · [IA aplicada](#ia-que-eu-construo-e-investigo) · [Tecnologias](#ecossistema-técnico) · [Contato](#vamos-conversar)

</div>

## Olá, eu sou Everton.

Sou **Engenheiro de Software e Professor de Tecnologia**. Há cerca de sete anos construo e evoluo software, principalmente com **Java/Spring Boot**, APIs e sistemas distribuídos. Gosto especialmente da parte que nem sempre aparece na demonstração: arquitetura, concorrência, integração entre serviços, qualidade, resiliência e manutenção ao longo do tempo.

Hoje aplico essa bagagem ao estudo e à construção de **sistemas com Inteligência Artificial** — de pipelines de RAG a workflows com agentes e ferramentas. Meu interesse não termina quando uma LLM produz uma resposta: quero entender o que acontece quando a aplicação precisa ser **segura, testável, observável e capaz de lidar com falhas**.

---

## Como eu penso engenharia

<img src="assets/engineering-map.svg" alt="Processo: entender o problema, desenhar a arquitetura, construir, validar e operar, considerando segurança, confiabilidade, custo e manutenção." width="100%" />

Não sou fã de arquitetura por moda. Prefiro partir das restrições do problema e justificar as escolhas:

| Desafio | O que procuro resolver |
| :--- | :--- |
| **Concorrência e consistência** | Proteger operações críticas com sincronização, semáforos e estratégias transacionais adequadas. |
| **Disponibilidade e desempenho** | Reduzir dependências e acessos desnecessários com cache-aside/Redis, sem ignorar invalidação e consistência. |
| **Modernização de legado** | Evoluir módulos com baixo risco, usando migração gradual e **Strangler Fig Pattern** quando faz sentido. |
| **Integração entre serviços** | Escolher contratos, mensageria e processamento assíncrono pensando em falhas, retries e observabilidade. |

**Minha referência é o comportamento do sistema em condições reais, não apenas o caminho feliz.**

---

## IA que eu construo e investigo

### 01 · IA aplicada ao ciclo de desenvolvimento

Participei da **evolução de um workflow corporativo de desenvolvimento assistido por IA, adotado pelo time de tecnologia**. Minha contribuição direta foi estruturar e implementar elementos de **Harness Engineering, Rules, Skills e Ralph Loop**, ampliando a autonomia dos ciclos de execução e validação.

Essa experiência alimenta meu interesse em **AI-assisted SDLC**, engenharia de contexto, documentação orientada por especificações, avaliações e limites claros para agentes. O workflow já existia antes da minha contribuição; meu foco foi **evoluir sua engenharia**.

### 02 · RAG e recuperação de conhecimento

Construí um pipeline funcional de ingestão de PDF, chunking, embeddings e busca semântica com **Python, LangChain, PostgreSQL e pgvector**. A aplicação utiliza trechos recuperados como contexto para responder perguntas e trata consultas sem evidência suficiente no documento.

[Explorar a implementação e os testes](https://github.com/EverttonFernandes/ingestao-busca-semantica-langchain-pgvector-postgresql)

### 03 · Laboratório de sistemas agênticos

Estou evoluindo um projeto autoral para estudar aplicações com **agentes, tool calling, RAG, estado de conversação, isolamento multi-tenant, idempotência, segurança e controle de custos**. A arquitetura e o roadmap também exploram **AI Gateway, evals, LLM-as-a-Judge e observabilidade**.

> **Em desenvolvimento:** o laboratório é uma plataforma de estudo e experimentação. Os temas citados incluem decisões de arquitetura e funcionalidades em construção; não representam uma operação comercial nem indicam que todos os componentes já estejam concluídos.

---

## Projetos com código

### [RAG · Ingestão e busca semântica em documentos](https://github.com/EverttonFernandes/ingestao-busca-semantica-langchain-pgvector-postgresql)

**Concluído · Python · LangChain · PostgreSQL/pgvector · Docker**

Como recuperar informação relevante de um documento e responder usando apenas o contexto encontrado? O projeto percorre ingestão, divisão em chunks, geração de embeddings, indexação e consulta por similaridade. Inclui testes de ingestão, recuperação e tratamento de respostas sem contexto.

### [Digital Bank API · Transações, contratos e concorrência](https://github.com/EverttonFernandes/Digital-Bank-API)

**Projeto de engenharia · Java 17 · Spring Boot 3 · PostgreSQL · Testes/CI**

API bancária construída para praticar decisões que importam além do CRUD: **transferências transacionais com lock pessimista**, semântica HTTP, HATEOAS, documentação OpenAPI, testes unitários e funcionais e validação por CI.

### [SOLID Principles Robots · Fundamentos explicados com código](https://github.com/EverttonFernandes/solid-principles-robots)

**Projeto didático · Java · Orientação a objetos**

Exemplos e material visual que usam robôs para explorar os princípios SOLID. Um encontro entre minha forma de projetar software e minha experiência ensinando programação.

### [Wishlist API · Contratos e testes funcionais](https://github.com/EverttonFernandes/wishlist-api)

**Projeto de backend · Java · Spring Boot · MongoDB · Jest**

API de lista de desejos para e-commerce, com operações de consulta e manutenção de itens, testes unitários e testes funcionais. Um exemplo de como exercitar **contratos de API e qualidade** em problemas menores.

---

## Ecossistema técnico

O que está abaixo reúne **experiência consolidada**, **prática aplicada** e **temas em aprofundamento** — sem tratar tudo como se tivesse o mesmo nível de vivência.

| Domínio | Minha caixa de ferramentas |
| :--- | :--- |
| **Backend & APIs** | `Java` · `Spring Boot` · `Python` · `FastAPI` · `REST` · `GraphQL` · `Node.js/TypeScript` |
| **Arquitetura** | `System Design` · `DDD` · `Microsserviços` · `Eventos` · `Concorrência` · `Resiliência` |
| **Data & Messaging** | `PostgreSQL` · `pgvector` · `MongoDB` · `Redis` · `Kafka` · `SQS/SNS` |
| **Quality & Operations** | `JUnit` · `Mockito` · `TDD/BDD` · `Docker` · `Kubernetes` · `CI/CD` · `Grafana` |
| **AI aplicada e em aprofundamento** | `LLMs` · `RAG` · `AI Agents` · `Tool Calling` · `Harness Engineering` · `Evals` · `AI Security` · `AI Gateway` |

<details>
<summary><b>Princípios que procuro levar para todos os projetos</b></summary>

- Requisitos e critérios de aceite claros antes de aumentar a complexidade.
- Decisões arquiteturais justificadas por contexto e trade-offs.
- Testes nas regras determinísticas; avaliações próprias para componentes probabilísticos.
- Observabilidade e segurança desde o desenho, não apenas após incidentes.
- Simplicidade quando ela resolve o problema — arquitetura distribuída quando há motivo real.

</details>

---

## Aprender, construir e compartilhar

Também sou professor de Tecnologia. Ensinar programação e orientar projetos reforçou algo que levo para o desenvolvimento: **entender um conceito de verdade é conseguir explicá-lo, questioná-lo e aplicá-lo**.

Gosto de estudar fundamentos, ler livros técnicos, experimentar abordagens novas e transformar o aprendizado em exemplos, projetos e discussões com outras pessoas. Estou cursando um **MBA em Engenharia de Software com Inteligência Artificial**, conectando essa formação à prática cotidiana.

---

## Vamos conversar

Se quiser trocar ideias sobre **engenharia de software, arquitetura, Java, Python, aplicações com LLMs, agentes ou aprendizado técnico**, será um prazer conectar.

[**GitHub**](https://github.com/EverttonFernandes) · [**LinkedIn**](https://www.linkedin.com/in/everton-oliveira-fernandes/)

<sub>Feito para evoluir junto com meus projetos. Sem widgets externos, sem métricas decorativas e sem promessas que o código não sustenta.</sub>
