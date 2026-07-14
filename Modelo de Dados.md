## Modelo de Dados

O projeto foi desenvolvido utilizando uma modelagem relacional otimizada para análise de vendas, seguindo o conceito de Star Schema.

### Tabelas

- **Clientes**: informações cadastrais dos clientes.
- **Produtos**: catálogo de produtos e preços.
- **Vendedores**: cadastro dos vendedores.
- **Vendas**: tabela de cabeçalho contendo cliente, vendedor e data da venda.
- **ItensVendas**: tabela fato contendo os itens vendidos, quantidade, descontos e valores.

### Relacionamentos

- Clientes (1) → (*) Vendas
- Vendedores (1) → (*) Vendas
- Vendas (1) → (*) ItensVendas
- Produtos (1) → (*) ItensVendas

### Diagrama
<img width="704" height="427" alt="modelo de dados" src="https://github.com/user-attachments/assets/b480e43c-d209-42a3-964f-02fa7dc8c98c" />
