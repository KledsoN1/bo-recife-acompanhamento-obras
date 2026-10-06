# 04 — Requisitos

> **Objetivo deste documento:** transformar a proposta de solução em requisitos claros e verificáveis.
>
> **Avaliação:** AV1 (revisar na AV2, se necessário)

---

## Requisitos funcionais

> Requisitos funcionais descrevem **o que o sistema deve fazer**. Escreva frases no formato "O sistema deve..." e evite termos vagos como "rápido" ou "fácil".

| ID | Requisito |
|---|---|
| RF01 | O sistema deve permitir o cadastro de obras públicas.|
| RF02 | O  sistema deve permitir a consulta das obras cadastradas.|
| RF03 |O sistema deve apresentar o andamento da obra. |
| RF04 |O sistema deve permitir visualizar os detalhes de uma obra. |
| RF05 |O sistema deve permitir que gestores atualizem informações das obras. |
| RF06 |O sistema deve disponibilizar uma área de consulta pública. |
| RF07 |O sistema deve apresentar informações financeiras da obra.|
| RF08 |O sistema deve apresentar indicadores sobre as obras no painel do gestor.|
| RF09 |O sistema deve apresentar informações financeiras da obra.|
| RF10 |O sistema deve apresentar a situação atual de cada obra.|
| RF11 |O sistema deve apresentar informações sobre prazos e datas.|



## Requisitos não funcionais

> Requisitos não funcionais descrevem **como** o sistema deve se comportar: qualidade, restrições e condições de operação. Sempre que possível, torne-os mensuráveis.

| ID | Categoria | Requisito |
|---|---|---|
| RNF01 | Segurança |O sistema deve exigir autenticação para o acesso às funcionalidades administrativas.|
| RNF02 | Usabilidade |O sistema deve apresentar as informações das obras de forma organizada e compreensível.|
| RNF03 | Desempenho |O sistema deve apresentar os resultados das consultas em até 3 segundos em condições normais de uso. |
| RNF04 | Acessibilidade |O sistema deve utilizar contraste adequado entre textos e elementos visuais.|
| RNF05 | Integridade |O sistema deve adaptar sua interface a diferentes tamanhos de tela.|
| RNF06 | Responsividade |O sistema deve manter os dados das obras armazenados corretamente após o cadastro ou atualização.|

## Critérios de aceite do MVP

> Critérios de aceite definem **quando o MVP pode ser considerado pronto**. Eles serão usados nos testes da AV2 ([08-testes-e-validacao.md](08-testes-e-validacao.md)).
>
> **Exemplo de formato (não é resposta):** "Dado que _[situação]_, quando _[ação do usuário]_, então _[resultado esperado]_."

- [ Dado que existam obras cadastradas, quando o usuário realizar uma pesquisa pelo nome ou identificador, então o sistema deve apresentar a obra correspondente aos dados informados.]
- [ Dado que uma obra esteja cadastrada, quando o usuário acessar seus detalhes, então o sistema deve apresentar informações como situação, andamento, prazo, localização e dados financeiros.]
- [Dado que o gestor tenha permissão para alterar uma obra, quando atualizar seus dados e salvar as alterações, então o sistema deve apresentar as informações atualizadas. ]
- [Dado que o cidadão acesse a área pública, quando consultar uma obra, então o sistema deve permitir visualizar suas principais informações sem necessidade de autenticação. ]
- [Dado que existam obras cadastradas com diferentes situações, quando o gestor acessar o painel, então o sistema deve apresentar indicadores relacionados às obras cadastradas.]
