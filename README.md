# Projeto: Gestão de Pedidos

## Dicionário de Dados

| Entidade | Atributo | Tipo | Tamanho| Descrição |
|-|-|-|-|-|
| Autor | id_autor | Inteiro | 11 | Identificador, PK, Auto incrementável |
| Autor | nome | varchar | 100 | Nome do autor |
| Autor | nacionalidade | varchar| 50 | Nacionalidade do autor |
| Autor | data_nascimento | date |  | Data de nascimento do autor |
| Livro | id_livro | Inteiro | 11 | Identificador do livro, PK, Auto incrementável |
| Livro | id_autor | Inteiro | 11 | Identificador do autor, FK, Auto referenciando Autor (id_autor) |
| Livro | titulo | varchar | 150 | Título do livro |
| Livro | isbn | varchar | 20 | Código ISBN do livro |
| Livro | ano_publicacao | Inteiro | 4 | Ano de publicação do livro|
| Livro | genero | varchar | 50 | Gênero literário do livbro |
| Livro | preco | Decimal | 10,2 | Preço do livro |
| Livro | estoque | Inteiro | 11 | Quantidade disponível no estoque |
| Cliente | id_cliente | Inteiro | 11 | Identificador do cliente, pk, Auto incrementável |
| Cliente | nome | varchar | 100 | Nome completo do cliente |
| Cliente | cpf | Inteiro | 11 | Quantidade do pedido |
| Cliente | email | varchar | 100 | E-mail do cliente  |
| Cliente | telefone | varchar | 20 | Número de telefone do cliente |
| Venda | id_venda | Inteiro | 11 | Identificador da venda, PK, Auto incrementável |
| Venda | id_cliente | Inteiro | 11 | Identificador do cliente, FK referenciando Cliente |(id_cliente)
| Venda | id_livro | Inteiro | 11 | Identificador do livro, FK referenciando livro (id_livro) |
| Venda | data_venda | date |  | Data em que a venda foi realizada | 
| Venda | quantidade | Inteiro | 11 | Quantidade de livros vendidos | 
| Venda | valor_total | Decimal | 10,2 | Valor total da venda | 

## Dados de teste em CSV
- [autor.csv](./autor.csv)
- [cliente.csv](./cliente.csv)
- [venda.csv](./venda.csv)
- [livro.csv](./livro.csv)


