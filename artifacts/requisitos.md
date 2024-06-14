## Requisitos

### Requisitos Funcionais

* **RF01. Cadastro Produtos**
  * Deve ser possível cadastrar, atualizar e remover produtos
  * Cada produto deve ter um nome, preço e pertencer a uma ou mais categorias
  * Deve ser possível aplicar diferentes descontos a cada produto em um pedido 
  * Produtos podem ser vendidos em múltiplas unidades
* **RF02. Cadastro de Categorias**
  * Deve ser possível cadastrar, atualizar e remover categorias
  * Produtos podem pertencer a várias categórias
* **RF03. Cadastro de Clientes** 
  * Deve ser possível cadastrar, atualizar e remover clientes 
  * Cada cliente deve ter nome, telefones, email, CPF ou CNPJ e um ou mais endereços 
  * Deve ser possível associar múltiplos endereços a um cliente 
  * Na hora do pedido, o cliente deve especificar o endereço de entrega
* **RF04. Gerenciamento de Pedidos**
  * Deve ser possível criar, atualizar e vesualizar pedidos 
  * Cada pedido pode conter um ou mais produtos, cada um com seu próprio desconto e quantidade 
  * Deve ser registrado o instante em que o pedido foi realizado
  * Deve ser especificado o endereço de entrega no momento do pedido
* **RF05. Gerenciamento de Pagamentos** 
  * Cada pedido deve ser pago por boleto ou cartão crédito 
  * No caso de pagamento por boleto, deve-se armazenar a data de vencimento e a data de pagamento 
  * No caso de pagamento por cartão de crédito, deve-se armarzenar o número de parcelas 
  * Cada pagamento deve ter um estado (pendente, quitado ou cancelado)
* **RF06. Relatórios e Consultas**
  * Consultar pedidos por cliente, data, estado do pagamento, etc
  * Relatórios de vendas por pedido, categoria de produto, etc

### Requisitos Não Funcionais

* **RNF01. Desempenho**
  * O sistema deve ser capaz de processar um grande número de pedidos simultaneamente
  * Consultas e relatórios devem ser gerados rapidamente, num tempo limite de 3 segundos
* **RNF02. Segurança**
  * Proteção de dados sensíveis, como informações de pagamento
  * Controle de acesso para diferentes perfis de usuários (administradores, vendedores, clientes, etc)
* **RNF03. Usabilidade**
  * Interface amigável e intuitiva para o usuário 
  * Facilidade na navegação e realização de operações como cadastro, atualização e consulta de dados
* **RNF04. Escalabilidade** 
  * O sistema de ve ser escalável para suportar um aumento no número de usuários e pedidos sem perda significativa de desempenho

### Considerações Finais 

O sistema deve ser desenvolvido com uma arquitetura que suporte expanções futuras e integração com outros sistemas, como gateways de pagamento e plataforma logística para entrega dos computadores. A segurança e privacidade dos dados dos clientes devem ser priorizadas, e o sistema deve estar em conformidade com a legislação LGPD (Lei Geral de Proteção de Dados)