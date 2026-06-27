### FinLend | Análise de Carteira de Crédito
O projeto simula o contexto de uma fintech de crédito pessoal (FinLend) e é estruturado em três partes: análise exploratória com Python, dashboard de self-service em Looker Studio e curadoria de um agente de IA generativa.

#### Estrutura do projeto
- `finlend_analise_carteira_credito.ipynb` — notebook principal com EDA, testes de hipótese, insight, recomendação ao negócio e validação do agente de IA
- [Dashboard Looker Studio](https://datastudio.google.com/reporting/4b719ea0-79e5-48f7-97fd-9db07f8c312f)

#### Contexto
A FinLend enfrenta três desafios simultâneos: falta de autonomia das áreas de negócio para consultar dados, aumento da taxa de inadimplência sem explicação clara e necessidade de validar um agente de IA antes de liberá-lo para uso interno.

#### Dataset
[Lending Club Loan Data](https://www.kaggle.com/datasets/wordsforthewise/lending-club) — dados reais de empréstimos P2P de 2007 a 2018. O arquivo completo contém 2.260.701 registros. Foi utilizada uma amostra aleatória de 150.000 registros, resultando em 89.192 empréstimos com desfecho conhecido após filtragem.

#### Parte 1 — Self-Service BI
Dashboard desenvolvido no Looker Studio com visão geral da carteira, indicadores de inadimplência, perfil dos tomadores e filtros interativos. A fonte de dados é uma amostra limpa exportada do notebook.

<img width="3750" height="3875" alt="FinLend___Carteira_de_Crédito_gif" src="https://github.com/user-attachments/assets/85053965-d585-4455-a871-31d1f49ca120" />

#### Parte 2 — Análise Estatística com Python
Análise exploratória completa da inadimplência com investigação da hipótese do Head de Risco ("a inadimplência está subindo porque estamos aprovando muitos empréstimos de graus D e E"), testes de hipótese (qui-quadrado, teste z de proporções e Mann-Whitney), insight não óbvio sobre seleção adversa via precificação e recomendação ao negócio.

**Stack:** Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy, Statsmodels

#### Parte 3 — Curadoria e Validação de IA Generativa
Validação quantitativa e qualitativa de uma resposta gerada por agente de IA sobre o perfil de risco do segmento de consolidação de dívidas, com proposta de melhoria e processo recorrente de validação.

#### Uso de IA assistiva
Este projeto foi desenvolvido com auxílio do Claude (Anthropic) para estruturação do código e organização do fluxo de trabalho. Todas as decisões analíticas foram tomadas e validadas por mim. Na Parte 3, o Claude deixa de ser ferramenta e passa a ser objeto da análise.
