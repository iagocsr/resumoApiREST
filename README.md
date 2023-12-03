# resumoApiREST


# API REST e RESTful

## Definição

API REST, ou Transferência de Estado Representacional, é um estilo de arquitetura para o desenvolvimento de sistemas distribuídos. Baseia-se em princípios que promovem escalabilidade, simplicidade e independência entre componentes, facilitando a comunicação entre sistemas.

## Principais Características

- **Sem Estado:** Cada requisição do cliente contém todas as informações necessárias para ser entendida e processada pelo servidor, sem que este mantenha qualquer estado da sessão do cliente entre requisições.
  
- **Recursos Identificáveis:** Os recursos, sejam dados ou serviços, são identificados por URLs, e a manipulação desses recursos é realizada por meio de operações HTTP padrão.

- **Representação dos Recursos:** Os recursos podem ter diferentes representações, como JSON ou XML, e o cliente pode negociar a representação desejada com o servidor.

## REST vs RESTful

- **REST:** É um estilo arquitetural que define princípios para projetar sistemas distribuídos.
  
- **RESTful:** Refere-se à aplicação efetiva dos princípios REST para o desenvolvimento de APIs, seguindo práticas e convenções do REST.

## Verbos HTTP

- **GET:** Obtém um recurso.
  
- **POST:** Cria um novo recurso.

- **PUT:** Atualiza um recurso existente.

- **DELETE:** Exclui um recurso.

- **PATCH:** Atualiza parcialmente um recurso.

## Códigos de Status HTTP

- **2xx (Sucesso):** Indica que a requisição foi bem-sucedida.

- **3xx (Redirecionamento):** Indica a necessidade de tomar ações adicionais para completar a requisição.

- **4xx (Erro do Cliente):** Indica um erro na requisição feita pelo cliente.

- **5xx (Erro do Servidor):** Indica que o servidor falhou ao realizar uma requisição válida.

## Exemplo Prático

### Requisição GET:

- **URI:** `/usuarios/123`

- **Resposta:** Retorna os detalhes do usuário com ID 123.

### Requisição POST:

- **URI:** `/usuarios`

- **Corpo:** `{ "nome": "João", "idade": 25 }`

- **Resposta:** Cria um novo usuário com as informações fornecidas.

### Requisição PUT:

- **URI:** `/usuarios/123`

- **Corpo:** `{ "nome": "João Silva" }`

- **Resposta:** Atualiza o nome do usuário com ID 123.

### Requisição DELETE:

- **URI:** `/usuarios/123`

- **Resposta:** Exclui o usuário com ID 123.

## Códigos de Status HTTP

- **200 OK:** Requisição bem-sucedida.

- **201 Created:** Recurso criado com sucesso.

- **204 No Content:** Requisição bem-sucedida, sem conteúdo para retornar.

- **400 Bad Request:** Requisição inválida do cliente.

- **404 Not Found:** Recurso não encontrado.

- **500 Internal Server Error:** Erro interno do servidor.
