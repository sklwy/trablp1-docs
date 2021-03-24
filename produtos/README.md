# Documentação Produtos
Cadastro de Produtos

## Modelo (Object)

### Comandas
Cadastro de Produtos

##### Rotas

*insert*: `"/api/produtos"` [`POST`]<br>
*listComandas*: `"/api/produtos/list` [`GET`]<br>
*findById*: `"/api/produtos/{proCod}` [`GET`]<br>

##### Campos 
| **CAMPOS** | **TIPO** | **TAMANHO** | **TRADUÇÃO** |<br>
| `proCod` | Long | 10 | Código |<br>
| `proDesNome` | Long | 10 | Descrição Produto |<br>
| `proIngrediente` | Array |  | Descrição Ingredientes |<br>
| `proValor` | Double | 255 |  | Valor Total de Produto |<br>