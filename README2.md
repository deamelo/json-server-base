Fake API atividade S3B11


O url base da API é https://json-server-base01.herokuapp.com/

# ENDPOINTS:

### REGISTRO:
Para efetuar o registro, será necessário o seguinte endpoint: 
 POST /register

No Body, email e password são obrigatórios para solicitação:
{
    "email": "kenzinho@mail.com",
    "password": "123456",
    "name": "Kenzinho",
    "age": 38,
  }


### LOGIN:
Para efetuar o login, será necessário o seguinte endpoint: 
  POST /login

No Body, email e password também serão necessários:
  {
    "email": "kenzinho@mail.com",
    "password": "123456",
  }


### CADASTRAR SEU PET:
O usuário deve estar logado para gravar o recurso e todos podem ler o recurso. 
*Necessário autorização via token.

Para cadastrar um pet, será necessário o seguinte endpoint: 
  POST /animails

No Body:
 {
	"species": "Gato",
	"name": "menina",
  "userId": 2
 }


### LER TODOS OS PETS:
Para buscar todos os pet, será necessário o seguinte endpoint: 
  GET /animails


### CADASTRAR E VISUALIZAR IDIOMAS:
O usuário deve estar logado para gravar o recurso e poder visualizar o recurso. 
*Necessário autorização via token.

Para buscar todos os idiomas cadastrados, será necessário o seguinte endpoint: 
  GET /languages


Para cadastrar um novo idioma, será necessário o seguinte endpoint: 
  POST /languages

No Body:
 {
	"languages": "Português",
  "userId": 2
 }






  