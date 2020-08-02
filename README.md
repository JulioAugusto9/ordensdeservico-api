# ordensdeservico-api
Api de ordens de Serviço feita com Spring Boot, Spring Web MVC, Spring Data, MySql, durante um treinamento online de Spring Rest para iniciantes ministrado pela AlgaWorks.

# Endpoints da API:
Adicionar o host na frente das rotas mostradas abaixo (por exemplo, se fizer o build localmente, adicionar "`http://localhost:8080`" antes de "/clientes" no caso da rota "Adicionar Cliente").
## Clientes:
### Adicionar Cliente
```json
POST /clientes


{
	"nome": "seuNome",
	"email": "seuEmail@provedor.com",
	"telefone": "99 99999-9999"
}
```
### Buscar Cliente
GET /clientes/{id}
### Listar Cliente
GET /clientes
### Atualizar Cliente
```html
PUT /clientes/{id}
```
```json
{
	"nome": "NomeAtualizado",
	"email": "EmailAtualizado@provedor.com",
	"telefone": "88 88888-8888"
}
```
### Excluir Cliente
DELETE /clientes/{id}
## Ordens de Serviço:
### Criar Ordem de Serviço
```json
POST /ordens-servico


{
	"cliente": {
		"id": 4
	},
	"descricao": "Reparo do pc Dell. Cliente diz que não liga.",
	"preco": 300.50
}
```
### Buscar Ordem de Serviço
GET /ordens-servico/{id}
### Listar Ordem de Serviço
GET /ordens-servico
### Finalizar Ordem de Serviço
PUT /ordens-servico/{id}/finalizacao
## Comentários nas Ordens de Serviço:
### Listar Comentários
GET /ordens-servico/{id}/comentarios
### Adicionar Comentário
```html
POST /ordens-servico/{id}/comentarios
```
```json
{
	"descricao": "Seu comentário a respeito desta ordem de serviço."
}
```
