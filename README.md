# Client-Serve_UDP-TCP
 
Código Java implementam comunicação cliente-servidor usando TCP e UDP.

### Cliente TCP (`TCPClient`)
1. O cliente TCP cria um socket para se conectar a um servidor TCP em um endereço IP e porta especificados.
2. Ele solicita uma entrada do usuário.
3. A entrada do usuário é enviada para o servidor.
4. O cliente recebe uma resposta do servidor e a imprime.

### Servidor TCP (`TCPServer`)
1. O servidor TCP cria um socket de recepção e aguarda conexões dos clientes.
2. Quando uma conexão é estabelecida, ele recebe a mensagem do cliente.
3. Ele converte a mensagem em maiúsculas.
4. O servidor envia a mensagem em maiúsculas de volta ao cliente.

### Cliente UDP (`UDPClient`)
1. O cliente UDP solicita uma entrada do usuário.
2. A entrada do usuário é enviada para o servidor usando datagramas UDP.
3. O cliente recebe uma resposta do servidor e a imprime.

### Servidor UDP (`UDPServer`)
1. O servidor UDP cria um socket para aguardar pacotes UDP na porta especificada.
2. Quando um pacote é recebido, ele converte o conteúdo em maiúsculas.
3. O servidor envia o conteúdo em maiúsculas de volta ao cliente.

### Considerações:
- O código TCP segue o padrão de um único envio e recebimento de dados por conexão.
- O código UDP segue um modelo de comunicação sem conexão, onde os pacotes podem ser perdidos ou entregues fora de ordem.
- Os códigos não lidam com tratamento de erros ou exceções, o que pode ser necessário em uma implementação real para garantir a robustez do sistema.
- As variáveis como "ip", "porta" e os números de portas (como "5040") precisariam ser substituídos pelos valores apropriados em uma aplicação real.
