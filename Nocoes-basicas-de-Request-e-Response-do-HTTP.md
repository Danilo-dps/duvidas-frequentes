					Noções básicas de Request e Response do HTTP
					
	Request (Requisição)

Uma requisição HTTP é um pedido enviado por um cliente (geralmente um navegador) para um servidor. Ela inclui:

    Método HTTP: Como GET, POST, PUT, DELETE. Cada um tem um propósito específico.

    URL: O endereço do recurso que você está solicitando.

    Headers: Metadados sobre a requisição, como Content-Type, Authorization, etc.

    Body: O conteúdo da requisição, usado principalmente em métodos como POST e PUT para enviar dados ao servidor.

Response (Resposta)

Uma resposta HTTP é a resposta do servidor ao cliente. Ela inclui:

    Status Code: Indica o resultado da requisição. Por exemplo, 200 para sucesso, 404 para recurso não encontrado, 500 para erro interno do servidor.

    Headers: Metadados sobre a resposta, como Content-Type, Content-Length, etc.

    Body: O conteúdo da resposta, que pode ser uma página HTML, dados JSON, arquivos, etc.

Exemplos:

    GET /api/users: Requisição para obter uma lista de usuários.

    POST /api/users com um corpo que contém dados do usuário: Requisição para criar um novo usuário.
