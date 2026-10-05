# 06 — Arquitetura e Tecnologias

> **Objetivo deste documento:** descrever como a solução será organizada tecnicamente e justificar as tecnologias escolhidas.
>
> **Avaliação:** AV1 (atualizar na AV2)
>
> **Não existe uma stack obrigatória.** Cada grupo pode escolher as tecnologias adequadas ao seu projeto. O importante é **justificar** a escolha e garantir que a equipe consegue entregar o MVP com ela.

---

## Arquitetura

O ObraFácil será uma aplicação web para acompanhamento de obras públicas. O sistema será composto por uma interface desenvolvida em HTML, CSS e JavaScript e um banco de dados SQLite para armazenamento das informações. Se possível, inclua um diagrama salvo em [`/assets`](../assets/)._

┌──────────────────────┐
│       USUÁRIO        │
│ Gestor / Cidadão     │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│       FRONTEND       │
│ HTML + CSS + JS      │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│    BANCO DE DADOS    │
│        SQLite        │
└──────────────────────┘

## Frontend

O frontend será desenvolvido com HTML5, CSS3 e JavaScript.

Será responsável pela interface e interação dos usuários com o sistema, incluindo:

Login;
Dashboard;
Cadastro de obras;
Listagem de obras;
Detalhes das obras;
Consulta pública.

## Backend

O projeto utilizará JavaScript para as funcionalidades e manipulação dos dados da aplicação.

A lógica será responsável por:

Cadastrar obras;
Consultar obras;
Atualizar informações;
Excluir registros;
Filtrar obras;
Exibir indicadores no dashboard.

## Banco de dados

Será utilizado o SQLite para armazenar os dados da aplicação.

O banco armazenará informações sobre:

Obras;
Responsáveis;
Empresas;
Orçamentos;
Cronogramas;
Status e progresso das obras.

## APIs

O MVP não utilizará APIs externas. A aplicação trabalhará com os dados armazenados no banco de dados SQLite.

## Serviços externos

O sistema não utilizará serviços externos no MVP, pois suas funcionalidades principais, como cadastro, consulta e acompanhamento das obras, serão desenvolvidas utilizando HTML, CSS, JavaScript e SQLite, sem necessidade de integração com serviços de terceiros.

## Infraestrutura

A aplicação será executada localmente durante o desenvolvimento, utilizando um servidor local para execução do projeto.

## Tecnologias

| Camada | Tecnologia | Justificativa |
|---|---|---|
| Frontend |HTML, CSS e JavaScript |Permitem desenvolver uma aplicação web simples, interativa e responsiva. |
| Backend |Não utilizado |O escopo do projeto não necessita de um backend separado. |
| Banco de dados |SQLite |Banco leve, simples e adequado ao armazenamento dos dados do projeto. |
| Hospedagem |Servidor local |Adequado para desenvolvimento e apresentação do MVP. |

## Justificativas técnicas

A escolha das tecnologias considera o escopo, prazo e conhecimento da equipe. HTML, CSS e JavaScript permitem desenvolver as principais funcionalidades do ObraFácil de forma simples e direta. O SQLite foi escolhido por ser um banco de dados leve e de fácil utilização, adequado ao volume de dados previsto para o projeto. A ausência de backend, APIs e serviços externos reduz a complexidade e facilita a implementação do MVP.

## Entidades principais

_Liste as principais entidades (dados) do sistema e seus atributos essenciais._

| Entidade | Atributos principais | Descrição |
|---|---|---|
|Obra|id, nome, descrição, categoria, município, bairro, endereço, status, percentual_execucao |Armazena as informações principais de cada obra pública. |
|Responsável|id, nome, órgão, contato|Identifica o responsável pelo acompanhamento da obra.|
|Empresa|id, nome, CNPJ, contato|Armazena os dados da empresa responsável pela execução da obra.|
|Orçamento|id, obra_id, valor_previsto, valor_executado|Armazena os valores financeiros relacionados à obra.|
|Cronograma|id, obra_id, data_inicio, data_prevista, data_conclusao|Armazena as informações relacionadas ao prazo de execução da obra.|
