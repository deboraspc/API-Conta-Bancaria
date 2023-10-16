# API-Conta-Bancaria

Conta Bancária, desenvolvida como parte de um projeto piloto para o Cubos Bank, o melhor banco digital do mundo. 
Esta API permite a gestão de contas bancárias, incluindo a criação de contas, consulta de informações de conta, 
depósitos, saques, transferências, consulta de saldo e geração de extrato bancário.

### Linguagens e Ferramentas

Node.js
Express.js

### Contribua com o projeto

- Realize o Fork
- Faça as modificações necessárias
- Realize a Pull Request (PR)

- ## :computer: Rodando o Projeto

-Certifique-se de ter o Node.js instalado.

-Clone o repositório
-Instale as dependências do projeto
-Inicie o servidor
-A API estará disponível em http://localhost:3000.

## Endpoints da API
###Listar Contas Bancárias
GET /contas?senha_banco=Cubos123Bank
Lista todas as contas bancárias existentes.

###Criar Conta Bancária
POST /contas
Cria uma nova conta bancária.

###Atualizar Usuário da Conta Bancária
PUT /contas/:numeroConta/usuario
Atualiza os dados do usuário de uma conta bancária.

###Excluir Conta
DELETE /contas/:numeroConta
Exclui uma conta bancária existente.

Requisição:

Número da conta bancária (passado como parâmetro na rota)

###Depositar
POST /transacoes/depositar
Realiza um depósito em uma conta bancária e registra a transação.

###Sacar
POST /transacoes/sacar
Realiza um saque em uma conta bancária e registra a transação.

###Transferir
POST /transacoes/transferir
Realiza uma transferência entre contas bancárias e registra a transação.

###Saldo
GET /contas/saldo?numero_conta=123&senha=123
Retorna o saldo de uma conta bancária.

### Extrato
GET /contas/extrato?numero_conta=123&senha=123
Lista as transações de uma conta bancária.
