
# Documentação Comandas
Cadastro de Comandas

## Modelo (Object)

### Comandas
Cadastro de Comandas

##### Rotas

*insert*: `"/api/comandas"` [`POST`]<br>
*listComandas*: `"/api/comandas/list` [`GET`]<br>

##### Campos 
| **CAMPOS** | **TIPO** | **TAMANHO** | **TRADUÇÃO** |<br><br>
| `comCod` | Long | 10 | Código |<br><br>
| `mesCod` | Long | 10 | Código Mesa |<br><br>
| `comPedidos` | Array |  | Lista de Pedidos |<br><br>
| `comValorTotal` | Double | 255 |  | Valor Total do Pedido |<br><br>
| `comDtaIni` | Date |  |  | Data Inicio/Hora |<br><br>
| `comDtaFini` | Date |  |  | Data Fim/Hora |<br><br>
| `comStatus` | String |  | ![datetime] | Status |<br><br>

##### ENUMs

###### EComStatus:
 `com.heroku.ifeslp1backend.enumerator.EComStatus`

* ATIVO
* FINALIZADO