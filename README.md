# Gabee — Documentação do projeto

Este repositório reúne a documentação de **produto, domínio, dados e decisões técnicas** da Gabee. Seu objetivo é registrar o raciocínio por trás do sistema e acompanhar a evolução do projeto, sem misturar documentação geral com detalhes específicos de frontend ou backend.

## Sobre o projeto

A Gabee está sendo explorada em duas frentes distintas:

- **Site / e-commerce:** catálogo de produtos personalizados, configuração de produtos e envio de solicitações de pedido para atendimento e produção. O acompanhamento detalhado dos pedidos é uma possibilidade futura.
- **Sistema de gestão interna:** possível plataforma para apoiar processos como pedidos, produção, insumos, custos e vendas. O escopo ainda precisa ser investigado e validado.

As duas soluções poderão se integrar no futuro, mas isso **não pressupõe** que precisem compartilhar a mesma arquitetura ou ser implementadas ao mesmo tempo.

## Estado atual

**Fase: descoberta e modelagem inicial.** O foco atual está em compreender as regras de negócio do site, definir conceitos do domínio e construir seu primeiro modelo de dados. As decisões documentadas são preliminares e poderão mudar conforme o aprendizado e a validação do produto.

Este trabalho também é um exercício prático de Engenharia de Software e uma possível preparação para um futuro projeto acadêmico. **Não constitui uma RFC oficialmente submetida ou aprovada.**

## Estrutura do repositório

| Caminho | Conteúdo |
| --- | --- |
| [`database/schema.dbml`](database/schema.dbml) | Modelo lógico inicial de dados, escrito em DBML. |
| `README.md` | Visão geral e orientações para a documentação. |

Outros documentos, como requisitos, regras de negócio, fluxos e decisões arquiteturais, serão adicionados conforme forem necessários.

## Como visualizar e atualizar o modelo de dados

1. Abra o arquivo [`database/schema.dbml`](database/schema.dbml).
2. Copie o conteúdo para o editor do [dbdiagram.io](https://dbdiagram.io/).
3. Faça os ajustes e valide as relações entre as tabelas.
4. Atualize o arquivo no repositório e registre a mudança em um commit.

O arquivo **DBML versionado neste repositório** é a referência para o *diagrama planejado*. Quando houver um banco implementado, as migrações aplicadas passarão a representar sua estrutura efetiva; a documentação deverá permanecer alinhada a elas.

## Tecnologias em estudo

- **Backend:** Java e Spring Boot.
- **Frontend:** React / Next.js e TypeScript.
- **Dados:** PostgreSQL, com Supabase como opção inicial de infraestrutura.

São direcionamentos atuais, **não decisões técnicas irreversíveis**.

## Princípio de trabalho

Priorizar um fluxo funcional e compreensível, validar necessidades reais, registrar decisões relevantes e evoluir a arquitetura conforme o problema exigir — evitando complexidade prematura.
