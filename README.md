# Crypto Genius - OLY
## Contrato AuctionCrypto - Contrato Inteligente de Leilão e Tokens
Este é um contrato inteligente desenvolvido em Solidity, que oferece funcionalidades para criar leilões e tokens para venda, facilitando a interação e transação de ativos digitais na blockchain. Pode ser feito deploy em qualquer EVM compativel.

## Funcionalidades

### Leilões
O contrato permite a criação e gerenciamento de leilões de ativos digitais. Os usuários podem criar leilões especificando o nome do item, preço inicial, duração do leilão e outras informações relevantes. Os participantes podem fazer lances durante o período do leilão, e o lance mais alto no final do período ganha o item em leilão.

### Tokens
Além dos leilões, o contrato também suporta a criação e transferência de tokens digitais. Os tokens podem representar ativos variados, como colecionáveis, recompensas ou direitos de participação em eventos. Os usuários podem criar novos tokens e transferi-los entre si conforme necessário.

### Pagamentos e Taxas
O contrato permite pagamentos em Ethereum para arrematar itens em leilões ou comprar tokens. Uma porcentagem do valor arrecadado nos leilões é retida como taxa de serviço, enquanto o restante é repassado ao vendedor do item. Da mesma forma, ao comprar tokens, uma parte do valor pode ser destinada ao proprietário do contrato como taxa de serviço.

## Como Usar

Para utilizar o contrato AuctionCrypto, siga estas etapas:
1. **Deploy do Contrato**: Deploy o contrato na blockchain Ethereum usando uma plataforma de sua escolha, como Remix ou executar esse projeto no Foundry.
Exemplo de como executar o Deploy na rede chiliz
`forge script script/AuctionCrypto.s.sol:AuctionCryptoScript --rpc-url chiliz --broadcast`
 2. **Interagir com o Contrato**: Utilize uma carteira Ethereum compatível, como MetaMask, para interagir com o contrato. Isso inclui criar novos leilões, fazer lances em leilões existentes, criar tokens e comprar tokens disponíveis.
3. **Gerenciar Transações**: Ao participar de leilões ou comprar tokens, certifique-se de ter saldo suficiente em sua carteira Ethereum. Além disso, esteja ciente das taxas associadas às transações, incluindo taxas de gás e taxas de serviço do contrato.
4. **Monitorar Atividades**: Acompanhe os eventos emitidos pelo contrato para monitorar a atividade dos leilões e transações de tokens. Isso inclui eventos como a criação de novos leilões, lances em leilões, encerramento de leilões e compra de tokens.

## Detalhe Técnico
### Contrato AuctionCrypto
O contrato AuctionCrypto é uma implementação em Solidity de um sistema de leilão e criação de tokens ERC721. Ele permite a criação e gerenciamento de leilões para itens específicos, bem como a criação e compra de tokens.

### Funcionalidades Principais:
+ function withdraw():
Função para o proprietário do contrato retirar os fundos acumulados no contrato.
+ function createAuction():
Permite a criação de um novo leilão para um item específico.
O criador do leilão pode especificar o nome, preço inicial e duração do leilão.
O item a ser leiloado é representado por um token ERC721.
+ function bid():
Usada pelos licitantes para fazer lances em um leilão.
Eles devem fornecer uma quantia de Ether maior do que o lance atual mais alto.
+ function endAuction():
Encerra um leilão depois que o tempo de duração especificado expira.
Determina o licitante vencedor e transfere o item leiloado para ele.
+ function getAllAuctions():
Retorna uma lista de todos os itens atualmente em leilão.
+ function getOwnerAuction(): 
Retorna uma lista de todos os itens em leilão que pertencem a um determinado endereço de carteira.
+ function createToken():
Permite a criação de um novo token ERC721.
O proprietário do contrato pode especificar o nome, valor inicial e metadados do token.
+ function purchaseToken():
Usada para comprar um token ERC721 disponível.
O comprador deve fornecer o valor especificado e recebe o token após a compra.
+ function getAllTokens():
Retorna uma lista de todos os tokens ERC721 criados.
+ function getOwnerTokens():
Retorna uma lista de todos os tokens ERC721 que pertencem a um determinado endereço de carteira.

