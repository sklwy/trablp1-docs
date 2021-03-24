# Documentação Comandas
Cadastro de Comandas

## Modelo (Object)

### Comandas
Cadastro de Comandas

##### Rotas

*insert*: `"/api/comandas"` [`POST`]<br>
*listComandas*: `"/api/comandas/list` [`GET`]<br>

##### Campos 
| **CAMPOS** | **TIPO** | **TAMANHO** | **TRADUÇÃO** |<br>
| `comCod` | Long | 10 | Código |<br>
| `mesCod` | Long | 10 | Código Mesa |<br>
| `comPedidos` | Array |  | Lista de Pedidos |<br>
| `comValorTotal` | Double | 255 |  | Valor Total de Comandas |<br>
| `comDtaIni` | Date |  |  | Data Inicio/Hora |<br>
| `comDtaFini` | Date |  |  | Data Fim/Hora |<br>
| `comStatus` | String | 15 |  | Status |<br>

##### ENUMs

###### EComStatus:
 `com.heroku.ifeslp1backend.enumerator.EComStatus`

* ATIVO
* FINALIZADO