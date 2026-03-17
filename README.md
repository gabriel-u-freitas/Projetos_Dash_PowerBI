# Portfólio Power BI 📊

Coleção de **dashboards desenvolvidos em Power BI** com foco na geração de insights a partir de cenários de negócio simulados.

Os projetos exploram **Power Query, modelagem de dados e criação de métricas em DAX**, com o objetivo de transformar dados brutos em informações acionáveis.

### Projetos

- [Dashboard Overview Parrot Technology](LINK)
- [Dashboard Comercial](LINK)

---

### Dashboard Overview Parrot Technology

![Demonstração do dashboard](GIF)

🔗 **Visualizar dashboard:** [Clique aqui](LINK)

#### Objetivo

Analisar movimentações financeiras para identificar padrões de receita e despesa, acompanhar a evolução das transações ao longo do tempo e entender a distribuição por bancos, tipo de movimentação e forma de pagamento.

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

- Valor total movimentado  
- Quantidade de transações  
- Distribuição por tipo de movimentação  
- Movimentações por banco  
- Evolução temporal das transações  

#### Ferramentas Utilizadas

- Power BI  
- Power Query  
- DAX  
- Excel  
