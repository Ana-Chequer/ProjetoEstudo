# ProjetoEstudo

Desenvolver uma solução para autorização de compras feitas em cartão de crédito. A solução deve contemplar tanto o lado servidor da solução quanto o cliente que fará as vezes do POS.

## Sobre as APIs:

- Criar uma API para solicitações de aprovação de compra;
- Considerar toda a lógica envolvida num processo de aprovação por exemplo, verificar se há saldo disponível, se a senha do usuário confere, se os dados da solicitação de autorização estão corretos, etc;
- A compra precisa ser registrada para consultas futuras;
- Todas as compras precisam ter um código de autorização único. As solicitações de autorização negadas também precisam ser registradas;
- Criar uma API que permita o cancelamento de compras dentro de um prazo de 30 dias a partir da data da compra;
- Criar uma API que forneça a lista das compras dos últimos X dias;
- Criar uma API que forneça a lista das compras da fatura Y;
- Criar uma API para informar o saldo do cliente;
- A API de aprovação de compra deve ser capaz de tratar regras de negócios que podem variar e/ou serem adicionadas e removidas a qualquer momento.
- Considerar como regras iniciais:
  - O saldo disponível;
Compras entre 22 Hs e 06 da manhã não podem ser maiores do que 20% do valor médias das compras desse cliente dos últimos 30 dias;
Todas as APIs precisam possuir Log;
Todas as APIs precisam expor métricas;
Todas as API's precisam ser documentadas com Swagger;


## Utilizar:
- Collections do Java;
- Swagger;
- Log4J ou similar;
- Micrometer;

## Estudar:
- Collections;
- Solid;
- Design Pattern State, Composite, Command, Facade
- Event Source, CQRS (ler superficialmente pois eu explicarei diretamente para agilizar)
