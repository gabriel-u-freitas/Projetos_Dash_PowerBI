# Portfólio Power BI 📊

Coleção de **dashboards desenvolvidos em Power BI** com foco na geração de insights a partir de cenários de negócio simulados.

Os projetos exploram **Power Query, modelagem de dados e criação de métricas em DAX**, com o objetivo de transformar dados brutos em informações acionáveis.

### Projetos

- [Dashboard Overview Parrot Technology](./Projeto%20Parrot%20Technology)
- [Dashboard Comercial](./Projeto%20Dashboard%20Comercial)

---

### Dashboard Overview Parrot Technology

![Demonstração do dashboard](./Projeto%20Parrot%20Technology/Demonstra%C3%A7%C3%A3o%20Parrot%20Technology.gif)

🔗 **Baixe o dashboard completo:** [Clique aqui](./Projeto%20Parrot%20Technology/Projeto%20Dashboard%20Parrot%20Technology.pbix)

#### Objetivo

Desenvolver um dashboard executivo completo para monitoramento integrado da performance comercial, contemplando indicadores de receita, volume de vendas, rentabilidade, atingimento de metas e participação de mercado. A solução também permite análises de ranking de clientes e produtos, incluindo análise de Pareto, além da simulação de cenários para avaliação de impactos em custos e margens.

#### Database

Base em **Microsoft Access** contendo variáveis que foram organizadas nas seguintes **tabelas Fato** e **tabelas Dimensão** (modelo no formato **Star Schema** para otimizar performance e facilitar análises em ferramentas de BI):

- fMeta [Ano, Mês, Valor Meta, País, Desc Categoria]
- fVendas [Pedido, Cod Cliente, Data Pedido, Data Faturamento, Cod Item, Quantidade, Desconto, Pagamento, Cod Tipo Venda]

- dCategoriaProduto [Cod Categoria, Descrição Categoria]
- dCliente [Cod Cliente, País, Estado, Cidade, Cod Funcionário]
- dComissao [Cod Funcionário, Percentual Comissão~]
- dFuncionarios [Cod Funcionário, País, Nome, Sobrenome, CPF, Data de Nascimento, Salário, Setor, Data de Admissão, Sexo, Cargo]
- dPais [ID Pais, Pais]
- dProduto [Cod Item, Preço Unitário, Custo Unitário]
- dSubCategoria [Cod Categoria, Cod Subcategoria, Subcategoria]
- dTipoVenda [Cod Tipo Venda, Descrição Tipo Venda]

#### Principais Métricas

💰 Financeiro
- Receita Soma  
- Receita Média  
- Receita Soma Brasil  
- Receita Soma LTM  
- Receita Soma YTD  
- Receita Soma YoY  
- Receita Soma YoY %  
- Receita Soma -1 Mês  
- Receita Soma -1 Mês crescimento %  
- Receita Soma sem Filtros Selecionados  
- Receita Soma Filtros Selecionados  
- Receita % total Filtros Selecionados  
- Receita % total sem Filtros Selecionados  
- Custos Soma  
- Lucro Bruto Soma  
- Margem Bruta  

📦 Vendas & Volume
- Vendas Qtd Soma  
- Vendas Qtd Média  
- Vendas Qtd Máx  
- Vendas Qtd Mín  
- Pedidos Qtd  
- Pedidos < 50k  
- Pedidos > 50K  
- Contratações  
- Clientes Qtd  

📈 Performance & Metas
- Meta Soma  
- Meta Soma YTD  
- Meta perfomance  
- Meta perfomance YTD  
- Máximo Velocímetro  
- Máximo Velocímetro YTD  

🌍 Mercado & Comparativos
- Market Share Brasil  
- Market Share ex-Brasil  
- Repres. vs Brasil  

🏆 Rankings & Análises
- Rank Categoria Produtos  
- Receita Soma Acumulada Rank Categoria Produtos  
- Receita Soma Acumulada Rank Categoria Produtos % total  
- Rank Clientes Geral  
- Rank Clientes Seleção  

🧪 Simulações & Cenários
- Simulação Custo Variação  
- Simulação Lucro Bruto  
- Simulação Margem Bruta  

#### Ferramentas Utilizadas

- Power BI  
- Power Query (linguagem M) 
- DAX  
- Microsoft Access

---

### Dashboard Comercial

![Demonstração do dashboard](./Projeto%20Dashboard%20Comercial/demonstracao%20sales%20perfomance%20analysis.gif)

🔗 **Baixe o dashboard completo:** [Clique aqui](./Projeto%20Dashboard%20Comercial/Projeto%20Dashboard%20Comercial%20-%20Prof.%20Omar%20Omar.pbix)

#### Objetivo

Desenvolver um dashboard para análise da performance de vendas, com foco na qualidade da receita, integrando indicadores de volume, faturamento, custos e rentabilidade. A solução permite avaliar o impacto financeiro de devoluções e descontos, além de analisar o desempenho por produto, categoria, marca e canal, apoiando a identificação de oportunidades de melhoria de margem.

#### Database

Base em **Excel**, não normalizada, contendo as variáveis:

- Data_venda
- Canal
- ProductKey
- Cod_Produto
- Desc_Produto
- Categoria_Produto
- Marca_Produto
- Classe_Produto
- Custo_Unit
- Preco_Unit
- Qtd_Venda
- Qtd_Devolução
- Valor_Devolução
- Qtd_Desconto
- Valor_Desconto

#### Principais Métricas

- Quantidade Vendida
- Receita Bruta
- Receita Líquida
- Custo
- Lucro Bruto
- Margem Bruta
- Quantidade de Devoluções
- Taxa de Devolução
- Impacto Financeiro Devoluções
- Taxa de Desconto Médio Concedido
- Impacto Financeiro Descontos

#### Ferramentas Utilizadas

- Power BI
- Power Query (linguagem M) 
- DAX  
- Excel
