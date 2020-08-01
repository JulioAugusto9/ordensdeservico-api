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
```json
GET /clientes
```
### Atualizar Cliente
PUT /clientes/{id}
```json
{
	"nome": "seuNome",
	"email": "seuEmail@provedor.com",
	"telefone": "99 99999-9999"
}
```
### Excluir Cliente
DELETE /clientes/{id}
## Ordens de Serviço:

