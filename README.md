# ordensdeservico-api
Api de ordens de Serviço feita com Spring Boot, Spring Web MVC, Spring Data, MySql, durante um treinamento online de Spring Rest para iniciantes.

Endpoints da API:

##Clientes
###Adicionar Cliente: 
POST http://HOST/clientes
{
	"nome": "seuNome",
	"email": "seuEmail@provedor.com",
	"telefone": "99 99999-9999"
}
