# Contrato Inteligente de Leilão e Tokens - Crypto Genius - OLY
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

1. **Deploy do Contrato**: Deploy o contrato na blockchain Ethereum usando uma plataforma de sua escolha, como Remix ou Truffle, ou executar esse projeto no Foundry.
### Exemplo de como executar o Deploy na rede chiliz
forge script script/AuctionCrypto.s.sol:AuctionCryptoScript --rpc-url chiliz --broadcast
 
2. **Interagir com o Contrato**: Utilize uma carteira Ethereum compatível, como MetaMask, para interagir com o contrato. Isso inclui criar novos leilões, fazer lances em leilões existentes, criar tokens e comprar tokens disponíveis.
3. **Gerenciar Transações**: Ao participar de leilões ou comprar tokens, certifique-se de ter saldo suficiente em sua carteira Ethereum. Além disso, esteja ciente das taxas associadas às transações, incluindo taxas de gás e taxas de serviço do contrato.
4. **Monitorar Atividades**: Acompanhe os eventos emitidos pelo contrato para monitorar a atividade dos leilões e transações de tokens. Isso inclui eventos como a criação de novos leilões, lances em leilões, encerramento de leilões e compra de tokens.


## Autor
Este contrato foi desenvolvido pela Equipe CryptoGenius.
Para mais informações, entre em contato com hackateam4@gmail.com.


## Equipe CryptoGenius
Dayana Mazini
UX/UI, Administradora, empreendedora com experiência no desenvolvimento de negócios inovadores nas áreas de finanças, educação e de transformação social.
LinkedIn: https://www.linkedin.com/in/dayanamazini/ 
Mazini.dayana@gmail.com

Aline Silva
Empreendedora, Atleta Olimpica, fundadora da Mempodera e da Firneza Token.
https://www.linkedin.com/in/influencer-aline-silva-oly
alinedaluta@gmail.com

Larissa Montefusco
Técnica em Eletrônica, Graduanda em Engenharia Eletrotécnica e de Computadores / Developer IoT e protocolos de comunicação, Django Python
https://www.linkedin.com/in/larissa-montefusco/
larissa.montefusco7@gmail.com

Sonia Mara Batista
Dev Blockchain, Solidity, Web3 
LinkedIn: https://www.linkedin.com/in/soniamarabatista/
dev.soniabatista@gmail.com

Matheus Oliveira
Desenvolvedor Flutter,  Fundador da Eita Rolê, empreendedor com experiência em desenvolvimento e impressão 3D.
LinkedIn: https://www.linkedin.com/in/devmatheusoliveira/
matheusoliveira.workmso@gmail.com
