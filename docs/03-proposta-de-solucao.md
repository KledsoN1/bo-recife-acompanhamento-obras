# 03 — Proposta de solução

> **Objetivo deste documento:** apresentar uma solução tecnológica proposta pela equipe e mostrar como ela se relaciona com o problema e as evidências levantadas.
>
> **Avaliação:** AV1
>
> Cada funcionalidade deve estar ligada a uma parte do problema descrito em [01-problema.md](https://github.com/KledsoN1/bo-recife-acompanhamento-obras/blob/main/docs/01-problema.md) e às evidências de [02-investigacao-e-evidencias.md](https://github.com/KledsoN1/bo-recife-acompanhamento-obras/blob/main/docs/02-investigacao-e-evidencias.md).

---

## Nome da solução

**ObraFácil**

## Resumo

O ObraFácil é uma plataforma web interativa voltada para o monitoramento e acompanhamento de obras públicas municipais. A solução centraliza informações sobre prazos, custos, andamento e responsáveis pelas obras. Para os gestores, facilita o acompanhamento e gerenciamento dos projetos. Para a população, oferece uma consulta pública simplificada e transparente sobre as obras do município.

## Público-alvo

- **Gestores públicos:** responsáveis pelo acompanhamento e gerenciamento das obras municipais.
- **População (cidadãos):** pessoas interessadas em consultar informações sobre as obras públicas do município.

## Usuários

| **Tipo de usuário** | **O que faz no sistema?** |
| ------------------- | ------------------------- |
| Gestor público | Cadastra, acompanha e gerencia informações sobre obras, prazos, custos, responsáveis e relatórios. |
| Cidadão | Consulta obras públicas e visualiza informações sobre andamento, custos, prazos, responsáveis e status da execução. |

## Proposta de valor

O ObraFácil centraliza as informações das obras públicas em uma única plataforma, tornando o acompanhamento mais organizado e facilitando a identificação de atrasos e custos adicionais.

Para os gestores, a solução oferece dashboards, indicadores e alertas para auxiliar no monitoramento das obras. Para a população, disponibiliza uma consulta pública simples e acessível, ampliando o acesso às informações sobre a execução dos projetos.

## Fluxo principal

### Gestor público

```text
Login
   ↓
Dashboard
   ↓
Lista de Obras
   ↓
Selecionar ou Cadastrar Obra
   ↓
Detalhes da Obra
   ↓
Relatórios
```

### Cidadão

```text
Consulta Pública
   ↓
Pesquisar ou Filtrar Obras
   ↓
Visualizar Obras
   ↓
Selecionar uma Obra
   ↓
Ver Detalhes
```

## Funcionalidades

| **ID** | **Funcionalidade**                | **Problema que ajuda a resolver**                                               | **Prioridade** |
| ------ | --------------------------------- | ------------------------------------------------------------------------------- | -------------- |
| F01    | Dashboard de acompanhamento       | Facilita o monitoramento de prazos, custos e status das obras pelos gestores.   | Alta           |
| F02    | Cadastro e gerenciamento de obras | Centraliza as informações das obras e reduz a dependência de processos manuais. | Alta           |
| F03    | Consulta pública de obras         | Facilita o acesso da população a informações claras sobre as obras públicas.    | Alta           |

## Funcionalidades futuras

- Atualização automática das informações das obras.
- Notificações sobre alterações no status das obras.
- Histórico de alterações e atualizações de cada obra.
- Integração com dados reais da Prefeitura.

## Diferencial

O ObraFácil integra, em uma única plataforma, o gerenciamento das obras pelos gestores públicos e a consulta transparente dessas informações pela população. A solução também prioriza uma interface simples e centrada no usuário, facilitando a navegação e o acesso às informações.
