Projeto de Portfólio: Dashboards de Vendas 2025 – Visão Geral da Performance

Esse case, segue o processo completo de análise de dados:
1. Definição Do Negócio 
1.1 PROBLEMA DE NEGÓCIO

Como aumentar a receita e a rentabilidade das vendas identificando os produtos, regiões e períodos que têm melhor desempenho?

1.2 PROBLEMA DE NEGÓCIO

	Descobrir quais produtos mais vendem.
	Identificar os clientes que mais compram.
	Avaliar sazonalidade (melhores meses).
	Medir lucratividade por produto, vendedor e região.
	Encontrar oportunidades para reduzir custos ou aumentar ticket médio.

1.3 PERGUNTAS DE NEGÓCIO


	Quais produtos geram mais receita?
	Quem São Os Top Vendedores Em Faturamento, Margem De Lucro E Ticket Médio?
	Qual região vende mais e qual tem menor lucro?
	Em que meses as vendas aumentam ou diminuem?
	Qual vendedor tem melhor conversão ou maior lucro?
	Quais produtos têm melhor margem de lucro?


Análise de dados não se começa no Power BI, mais sim no nosso Banco.
SQL é a habilidade que dá autonomia para o analista gerar N Insights, onde Planilha é cálculo e Banco de dados é informação.
Para a Estrutura da nossa Query, usamos os seguintes Comandos: 

Comando de agregações
CTE com a clausula With
Funções de Janelas 
Joins
Etc...


<img width="1145" height="829" alt="image" src="https://github.com/user-attachments/assets/d93c800f-6b09-4351-9faf-f909321f5d7e" />

<img width="1168" height="1540" alt="image" src="https://github.com/user-attachments/assets/f68946b5-f327-4a03-bedd-66eb24bf58f3" />
<img width="1150" height="1498" alt="image" src="https://github.com/user-attachments/assets/326cccbe-22f5-4a07-97b3-640744dedc8c" />


O Nosso Power BI, Será A Consequência Da Nossa Análise Mais Visual 

2. Coleta Dos Dados
Fonte dos Dados:
Os dados foram obtidos do Banco comercio 3 onde Compõem:
A Tabela Base Venda:
 Data Venda, Produto, Região, Vendedor, Quantidade, Preço Unitário, Custo Unitário, Receita e Lucro

<img width="886" height="434" alt="image" src="https://github.com/user-attachments/assets/ca660ee5-ec66-45af-9094-b96d4a76b36c" />

3. Ferramentas Utilizadas 
Usei Power Query para:
3.1 Importação, Limpeza e Tratamento (ETL com Power Query)
Tarefas realizadas:
Remoção de linhas em branco e duplicadas
Padronização de datas e nomes
Criação de colunas calculadas:
Custo = Quantidade × Custo Unitário
Criação de colunas de Mês e Ano

 4. Modelagem de Dados: Relacionamentos e estrutura Star Schema.

Explicação Clara:
Usei Modelagem Dimensional, Criando a tabela Fato e Dimensão para facilitar o nosso relacionamento entre as tabelas. 
A normalização para dividir   a nossa tabela, evitando assim a redundância nas nossas informações. 

Modelo em estrela (Star Schema):
             Dim_Vendedor
                  |
 Dim_Produto — Fato_Venda — Dim_Região
                  |
             Dim_d_Calemdario 

3. Ferramentas Utilizadas 
Usei Power Query para:
3.1 Importação, Limpeza e Tratamento (ETL com Power Query)
Tarefas realizadas:
Remoção de linhas em branco e duplicadas
Padronização de datas e nomes
Criação de colunas calculadas:
Custo = Quantidade × Custo Unitário
Criação de colunas de Mês e Ano

 4. Modelagem de Dados: Relacionamentos e estrutura Star Schema.

Explicação Clara:
Usei Modelagem Dimensional, Criando a tabela Fato e Dimensão para facilitar o nosso relacionamento entre as tabelas. 
A normalização para dividir   a nossa tabela, evitando assim a redundância nas nossas informações. 

Modelo em estrela (Star Schema):
             Dim_Vendedor
                  |
 Dim_Produto — Fato_Venda — Dim_Região
                  |
             Dim_d_Calemdario 

3. Ferramentas Utilizadas 
Usei Power Query para:
3.1 Importação, Limpeza e Tratamento (ETL com Power Query)
Tarefas realizadas:
Remoção de linhas em branco e duplicadas
Padronização de datas e nomes
Criação de colunas calculadas:
Custo = Quantidade × Custo Unitário
Criação de colunas de Mês e Ano

 4. Modelagem de Dados: Relacionamentos e estrutura Star Schema.

Explicação Clara:
Usei Modelagem Dimensional, Criando a tabela Fato e Dimensão para facilitar o nosso relacionamento entre as tabelas. 
A normalização para dividir   a nossa tabela, evitando assim a redundância nas nossas informações. 

Modelo em estrela (Star Schema):
             Dim_Vendedor
                  |
 Dim_Produto — Fato_Venda — Dim_Região
                  |
             Dim_d_Calemdario 


<img width="1152" height="638" alt="image" src="https://github.com/user-attachments/assets/5127f73a-6d5a-447b-81fa-2f110737883c" />



 5. DAX: Medidas, indicadores e KPIs.
5.1 Métricas 
•	Total vendido (Medir tamanho do negócio)
•	Total de custo
•	Total de lucro (Medir eficiência)
•	Quantidade vendida

5.2  Indicadores 
•	Ticket Médio = Receita ÷ Nº pedidos (Monitorar valor de vendas por transação)
•	Margem de Lucro (%) = Lucro ÷ Receita × 100 (Objetivo Avaliar saúde financeira)
•	Crescimento Anual (%) :Objetivo é avaliar o crescimento ano a ano (YOY) 

5.3  KPIs Estruturados com os Seguintes Gráficos e Tabelas 
•	Receita por mês e ano 
•	Receita por produto 
•	Custo por produto
•	Lucro por produto
•	Tabela que ilustra o comparativo anual como: ano, faturamento, crescimento ano, lucro, margem de lucro e ticket médio
•	Lucro por região
•	Faturamento por região 
•	Crescimento anual por região 
•	Tabela que apresenta as seguintes analises dos produtos: Faturamento, lucro, margem de lucro e ticket médio
•	Tabela que ilustra a performance por vendedores: Faturamento, lucro, margem de lucro e ticket médio
•	Tabela que monstra a margem de lucro por produto em cada região: Nome produtos, regiões e margem de lucro 


<img width="1129" height="1104" alt="image" src="https://github.com/user-attachments/assets/5ebe69c8-40a1-450b-915f-6dfda20371c7" />


6. Visualização: Gráficos, tabelas dinâmicas e layout.
Elementos do Dashboard:
Card: para mostrar um único valor criando assim impacto rápido.
Gráfico de Linha:  Ideal para mostrar tendências ao longo do tempo 
Gráfico de Barra: Usamos para comparar categorias 
Gráfico de Coluna: Usamos para comparar categorias 
Tabela dinâmica: Usamos porque resumo grande volume de dados que permite agrupar com mais eficiência. 

<img width="1125" height="802" alt="image" src="https://github.com/user-attachments/assets/c9af3cec-62b3-47eb-80e4-2cbd15669a59" />

<img width="1035" height="645" alt="image" src="https://github.com/user-attachments/assets/de938a69-2775-4f08-920c-d3d9186ab9bd" />

<img width="1060" height="688" alt="image" src="https://github.com/user-attachments/assets/df6b48ee-79be-44d7-a61d-646eff262174" />

<img width="1121" height="697" alt="image" src="https://github.com/user-attachments/assets/a3fea6a0-773d-48b2-9e92-2b3e3270d49a" />

<img width="1108" height="678" alt="image" src="https://github.com/user-attachments/assets/bd33ae74-77c5-406f-a619-1ad22e28338f" />




