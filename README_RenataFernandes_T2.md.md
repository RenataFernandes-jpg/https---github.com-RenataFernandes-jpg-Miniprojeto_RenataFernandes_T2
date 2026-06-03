# Miniprojeto SCTEC

A base “Varejo” extraída do KAGGLE contém registros reais de compras (datas, clientes, produtos, categorias e valores). Vamos verificar a
qualidade, limpar e sumarizar esses dados.
Neste mini-projeto vamos identificar os problemas nos dados (valores nulos, tipos incorretos, duplicados), 
tratar esses problemas com ferramentas como pandas e gerar estatísticas  simples e funções de agrupamento, 
para responder perguntas operacionais.

Problemas de dados identificados na base:
valores nulos na coluna categoria que usei a função replace para atualizar para outros por ter receita.
Linhas duplicadas excluídas
Conversão de data com o datetime

#### Estatísticas descritivas básicas para coluna de número de filhos do cliente:

|Name: CL_FHL    |dtype: str|
| ---: | ---: |
|count    |733,447.00|
|mean     |      1.15|
|std      |      1.42|
|min      |      0.00|
|25%      |      0.00|
|50%      |      0.00|
|75%      |      2.00|
|max      |      4.00|

#### Perguntas operacionais:

#### Quem compra mais?

Através da análise exploratória identificamos que as mulheres compras mais, conforme mostra o gráfico abaixo:

  <div>
    <img width="382" height="404" alt="Image" src="https://github.com/user-attachments/assets/a9b4a1ac-29d1-4392-b9f4-2f39d5b3e9cc" />
  </div>
  
#### Quais categorias vendem mais?

A categoria alimentos a que mais vende.

  <div>
    <img width="890" height="390" alt="Image" src="https://github.com/user-attachments/assets/aa917e29-a9bb-44d0-b51f-a43693c4eaca" />
  </div>
  
#### Como variam as vendas ao longo do tempo?

As vendas seguem crescendo de 2019 ate 2021, porém a vendas caem em 2022 e a categoria que mais perdeu receita foi a de alimentos.

 <div>
    <img width="590" height="490" alt="Image" src="https://github.com/user-attachments/assets/862ad0ab-3dcb-4449-a9fc-02ec913885bf" />
  </div>

| Categoria | 2019 | 2020 |2021 |2022 |
| :--- | :---: | ---: | ---: | ---: |
| ACESSORIOS | R$ 0.29M |  R$ 0.32M |  R$ 0.35M | R$ 0.25M|
| ALIMENTOS  | R$ 9.69M | R$ 10.65M | R$ 11.98M | R$ 8.13M|
| BEBIDAS    | R$ 1.00M |  R$ 1.12M |  R$ 1.23M | R$ 0.84M|
| HIGIENE    | R$ 4.13M |  R$ 4.51M |  R$ 5.07M | R$ 3.44M|
| LIMPEZA    | R$ 4.18M |  R$ 4.56M |  R$ 5.10M | R$ 3.49M|
| OUTROS     | R$ 0.08M |  R$ 0.09M |  R$ 0.10M | R$ 0.07M|
| PET        | R$ 0.89M |  R$ 0.98M |  R$ 1.10M | R$ 0.75M|

