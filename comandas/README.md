
# Documentação Comandas
Cadastro de Comandas

## Modelo (Object)

### Comandas
Cadastro de Comandas

##### Rotas

*insert*: `"/api/comandas"` [`POST`]<br>
*listComandas*: `"/api/comandas/list` [`GET`]<br>

##### Campos 
| **CAMPOS** | **TIPO** | **TAMANHO** | **TRADUÇÃO** | 
|--|--|--|--|--|
| `comCod` | Long | 10 | Código |
| `mesCod` | Long | 10 | Código Mesa |
| `comPedidos` | Array |  | Lista de Pedidos |
| `comValorTotal` | Double | 255 |  | Valor Total do Pedido |
| `comDtaIni` | Date |  |  | Data Inicio/Hora |
| `comDtaFini` | Date |  |  | Data Fim/Hora |
| `comStatus` | String |  | ![datetime] | Status |

##### ENUMs

###### EComStatus:
 `com.heroku.ifeslp1backend.enumerator.EComStatus`

* ATIVO
* FINALIZADO