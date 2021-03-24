# Documentação Pedidos
Cadastro de Pedidos

## Modelo (Object)

### Pedidos
Cadastro de Pedidos

##### Rotas

*insert*: `"/api/pedidos"` [`POST`]<br>
*listPedidos*: `"/api/pedidos/list` [`GET`]<br>
*findById*: `"/api/pedidos/{pedCod}` [`GET`]<br>

##### Campos 
| **CAMPOS** | **TIPO** | **TAMANHO** | **TRADUÇÃO** |<br>
| `pedCod` | Long | 10 | Código |<br>
| `comCod` | Long | 10 | Código Comandas |<br>
| `proCod` | Long | 10 | Código Produto |<br>
| `pedStatus` | String | 15 |  | Status |<br>
| `pedVlrTotal` | Date |  |  | Valor Total de Pedido |<br>
| `pedMemObs` | Date |  |  | Observação Pedido |<br>

##### ENUMs

###### EComStatus:
 `com.heroku.ifeslp1backend.enumerator.EPedStatus`

* ATIVO
* CANCELADO
* FINALIZADO