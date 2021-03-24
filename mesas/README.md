[invisible]:/uploads/9216957cf1fb0499c3d1189e107e0e88/-INVISIBLE-GRAY.svg
[insert]:/uploads/e4432d0bb73c1578ba12b8ceb89a86c1/-INSERT-B09C09.svg
[delete]:/uploads/05be2821166b825e9c7deeba5f67839a/-DELETE-1A0C4A.svg
[update]:/uploads/31b9339a410ab382e57be40eeea515b1/-UPDATE-FF5737.svg
[lov]:/uploads/8dbb1de071297eb94d3f46cc279b6999/-LOV-A115FF.svg
[main]:/uploads/d640813b47af66d915d74a55a256dc5a/-MAIN-brightgreen.svg
[required]:/uploads/9585bb5470e39990e6a8276338a85504/-REQUIRED-red.svg
[datetime]:/uploads/656befd24cd9263985c427940104a50d/-DATETIME-0D6B44.svg
[enum]:/uploads/95c06c1b6c0d952563159e5d4df3a275/-ENUM-001AE8.svg

# WRK001
Cadastro de Situação de Tarefas

## MODELOS

### ComSituacaoTarefa
Cadastro de Situação de Tarefas

##### Rotas

*update*: `/api/wrk001/` [`PUT`]<br>Filters:`{}` <br>
*insert*: `/api/wrk001/` [`POST`]<br>Filters:`{}` <br>
*findById*: `/api/wrk001/{stfCod}` [`GET`]<br>Filters:`{}` <br>
*getList*: `/api/wrk001/list` [`POST`]<br>Filters:`{}` <br>
*getLogList*: `/api/wrk001/log/{stfCod}` [`GET`]<br>Filters:`{}` <br>
*cancelaRegistro*: `/api/wrk001/cancelar` [`PUT`]<br>Filters:`{}` <br>
*delete*: `/api/wrk001/{stfCod}` [`DELETE`]<br>Filters:`{}` <br>

##### Campos 
| **FIELD** | **TYPE** | **SIZE / PRECISION** | **MODIFIERS** | **TRANSLATION** | 
|--|--|--|--|--|
| `stfCod` | Long | 10 | ![required] | Código |
| `stfDesNome` | String | 50 |  | Descrição da Situação da Tarefa |
| `stfVldStatus` | Long |  |[![enum]](#stfvldstatus)    | Status |
| `usnCodCad` | Long | 10 |  | Cod. Usuário |
| `usnDesNomeCad` | String | 50 |  | Nome do Usuário Cadastrado |
| `usnDesNomeStatus` | String | 50 |  |  |
| `stfTimCad` | Date |  | ![datetime] | Data/Hora Cadastro |
| `usnCodStatus` | Long | 10 |  |  |
| `stfTimStatus` | Date |  | ![datetime] |  |
| `stfVldFechamento` | Long |  |[![enum]](#stfvldfechamento)    | Indica Fechamento ? |

##### ENUMs

###### stfVldStatus:
 `info.conexos.model.enumVld.EAtivoCancelado`

* (1)ATIVO - ATIVO
* (2)CANCELADO - CANCELADO 

###### stfVldFechamento:
 `info.conexos.model.enumVld.ESimNao`

* (0)NAO - NÃO
* (1)SIM - SIM 
