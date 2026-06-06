# Miniprojeto SCTEC

A base “Varejo” extraída do KAGGLE contém registros reais de compras (datas, clientes, produtos, categorias e valores). Vamos verificar a
qualidade, limpar e sumarizar esses dados.
Neste mini-projeto vamos identificar os problemas nos dados (valores nulos, tipos incorretos, duplicados), 
tratar esses problemas com ferramentas como pandas e gerar estatísticas  simples e funções de agrupamento, 
para responder perguntas operacionais.

#### Perguntas operacionais:

Quem compra mais?

Qual segmento compra mais?

Quais categorias vendem mais?

Como variam as vendas ao longo do tempo?

#### Problemas de dados identificados na base:

Valores nulos na coluna categoria que usei a função replace para corrigir.

Linhas duplicadas excluídas.

Conversão de data com o datetime.

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


#### Respostas para as perguntas operacionais:


#### Clientes

Através da análise exploratória identificamos que as mulheres são responsáveis por 52% das vendas

  <div>
    <img width="382" height="404" alt="Image" src="https://github.com/user-attachments/assets/718a8e24-6def-487e-8a3e-0973b1b92eb3" />
  </div>

#### Segmentos

Cerca de 64% da base esta concentrado no segmento B

  <div>
    <<img width="382" height="404" alt="Image" src="https://github.com/user-attachments/assets/d6a1fd79-7047-446a-b925-e32034e1160b" />
  </div>

  
#### Categorias

As categorias alimentos representam 52% dos produtos vendidos

 <div>
    <img width="428" height="404" alt="Image" src="https://github.com/user-attachments/assets/7707cc06-cbf0-4465-8e30-d77146963078" />
  </div>

  
#### Vendas

A quantidade de produtos vendidos seguem crescendo de 2019 até 2021, porém a vendas caem em 2022 e a categoria que mais diminuiu nas suas vendas foi a de alimentos.

 <div>
    <img width="590" height="490" alt="Image" src="https://github.com/user-attachments/assets/68e339d9-b9d6-417f-9a26-c1bf23292e7a" />
  </div>


| Categoria | 2019 | 2020 |2021 |2022 |
| :--- | :---: | ---: | ---: | ---: |
| ALIMENTOS  |92K | 101K| 114K|  77K|
| HIGIENE    | 33K| 36K |  41K|  28K|
| LIMPEZA    | 31K|  34K|  38K|  26K|
| BEBIDAS    | 9K | 10K |  11K|   8K|
| ACESSORIOS | 3K | 3K  |  3K |   4K|
| OUTROS     | 1K |   1K|   1K|   1K|
| PET        | 7K |   8K|   8K|   6K|

