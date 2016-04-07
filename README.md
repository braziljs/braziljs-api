## BrazilJS APIs

A BrazilJS possui uma API que te permite consultar algumas informações relevantes por meio de requisições GET.

### Endereço

Para usar a API, utilize o endereço:

`https://braziljs.org/api/[command]`

Onde [command] pode ser um dos serviços listados abaixo:

### Eventos

Comando: `list/events`<br/>
Variáveis: `fromNow`<br/>
Retorno: Um JSON com a lista de eventos do ano atual.<br/>
Caso a variável `fromNow` seja enviada com valor 1, trará apenas eventos a partir da data atual.

Exemplo:

`https://braziljs.org/api/list/events?fromNow=1`

### Artigos

Comando: `list/articles`<br/>
Variáveis: N/A<br/>
Retorno: Um JSON contendo a lista dos últimos 10 artigos.

### Patrocinadores

Comando: `list/sponsors`<br/>
Variáveis: `eventId`<br/>
Retorno: Um JSON com a lista de patrocinadores do programa de afiliados BrazilJS.<br/>
Caso a ID de algum evento seja enviada, retorna apenas os patrocinadores para aquele evento.

Exemplo:

`https://braziljs.org/api/list/sponsors?eventId=56979ef67dd947993c745f26`

Retornará um `json` com a lista de patrocinadores do evento BrazilJS 2016.



