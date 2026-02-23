## Blockchain 

- [x] **Fundamentos de Blockchain (Material do Muriel):**
	1. Entender o que realmente importa para implementar
	2. Como funciona um bloco (hash, nonce, Merkle Tree)
	3. Diferença entre -> Blockchain pública (Ethereum) e privada (Hyperledger Fabric)
	4. O que são smart contracts

- [x] Solidity na prática (mínimo necessário)
	1. Saber criar e interagir com smart contracts
	2. Estrutura de um smart contract
	3. `struct, mapping, event`
	4. Controle de acesso (`modifier`, `onlyOwner`)
	5. Deploy + testes no Remix/Ganache
	6. Exercício mínimo: 
		- Contrato que registra um dado (hash de um prontuário, por exemplo)
		- Emite evento
		- Controla quem pode escrever
		- Neste caso Solidity não é o core, é um meio.

- [x] Go e Blockchain (Frameworks e implementações)
	1. Estudar sobre `go-ethereum (geth)`
	2. Gerar binding Go a partir de contratos Solidity (`abigen`)
	3. Criar:
		- API em Go que interage com contratos
		- Serviço que registra e consulta dados na blockchain
	4. Go + Hyperledger Fabric -> https://www.youtube.com/watch?v=eRCEaUZz5ZU&list=PLcbbqdJgPgcXlRlPNHF2itTotEwr9kckl&index=28
		- Chaincode pode ser escrito em Go
		- Ideal para: Dados sensíveis, controle de acesso, blockchain privada (hospital, clínica e laboratório)
		- Trabalhar com chaincode (smart contracts em Go)
		- MSP (identidade)
		- Canais privados
		- Políticas de endosso

- [ ] Saúde + Blockchain
	1. LGPD, confiabilidade, auditabilidade, imutabilidade, compartilhamento seguro de informações.
	2. Nunca armazenar o prontuário eletrônico na blockchain, apenas:
		- Hash
		- Metadados
		- Controle de acesso
		- Referências a dados off-chain

