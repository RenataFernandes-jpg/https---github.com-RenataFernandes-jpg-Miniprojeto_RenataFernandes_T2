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

Através da análise exploratória identificamos que as mulheres compram mais do que os homens, conforme mostra o gráfico abaixo:

  <div>
    <img width="382" height="404" alt="Image" src="https://github.com/user-attachments/assets/718a8e24-6def-487e-8a3e-0973b1b92eb3" />
  </div>
  
#### Quais categorias vendem mais?

As categorias alimentos, higiene e limpeza são as que mais vendem. 

 <div>
    <img width="989" height="490" alt="Image" src="https://github.com/user-attachments/assets/04399749-b4cd-4251-94c8-f219f0f9e9ad" />
  </div>
  
#### Como variam as vendas ao longo do tempo?

A quantidade de produtos vendidos seguem crescendo de 2019 ate 2021, porém a vendas caem em 2022 e a categoria que mais diminuiu nas suas vendas foi a de alimentos.

 <div>
    <img width="590" height="490" alt="Image" src="https://github.com/user-attachments/assets/68e339d9-b9d6-417f-9a26-c1bf23292e7a" />
  </div>

| Categoria | 2019 | 2020 |2021 |2022 |
| :--- | :---: | ---: | ---: | ---: |
| ACESSORIOS | 3K | 3K  |  3K |   4K|
| ALIMENTOS  |92K | 101K| 114K|  77K|
| BEBIDAS    | 9K | 10K |  11K|   8K|
| HIGIENE    | 33K| 36K |  41K|  28K|
| LIMPEZA    | 31K|  34K|  38K|  26K|
| OUTROS     | 1K |   1K|   1K|   1K|
| PET        | 7K |   8K|   8K|   6K|

