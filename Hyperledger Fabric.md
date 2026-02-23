- [[Fundamentos de Blockchain#**Tipos de Blockchain**|É uma blockchain open-source, permissionada]].
- Mantida pela Linux Foundation
- Blockchain permissionada:
	1. Somente pessoas autorizadas podem participar da rede.
	2. Participantes são conhecidos e identificados
	3. Há regras de quem pode ler, escrever ou validar transações.
	4. A identidade é verificada por certificados digitais.
	5. O consenso é mais eficiente (não usa mineração), [[Fundamentos de Blockchain#**Mecanismos de consenso**|Proof of Authority]].

- Utiliza-se de chaincodes (smart contracts) com linguagens como Go, NodeJs e Java.
- Mecanismos de consenso --> Por padrão utiliza o [[CFT (Crash Fault Tolerance)|Raft (CFT)]].

### Organização 
- Redes que podem ser independentes
- Contêm os nós e podem possuir uma aplicação própria
### Canais 
- Canais de comunicação entre nós de distintas organizações.
- Garantem a privacidade dos dados.
- Nós podem participar de vários canais.

![[Pasted image 20260223185410.png]]

### Organizações da rede
- Principais tipos de nós
	1. **Cliente:** 
		- Atua em nome do usuário final
	2. **Peer (nó validador):**
		- Hospeda a ledge, executa os contratos inteligentes e valida as transações
		- Pode ou não ser de endosso (endorsing peer), o qual simula a transação em cima do seu ledger atual, gerando o read/write set (*i.e.* o que deve ser mudado)
	3. **Ordenador (ordering)**:
		- Verifica as políticas das transações recebidas (e.g. se todos os nós de endosso devem assinar, isso aconteceu?)
		- Verifica se os read/write sets recebidos dos nós de endosso batem
		- Ordena as transações recebidas utilizando o mecanismo de consenso
		- Gera e distribui blocos

### Autoridade certificadora (certificate authority, CA)
- Permite a identificação de usuários, nós e organizações
- Todos os nós validam as assinaturas recebidas, realizam suas tarefas e assinam o resultado antes de passá-lo adiante.

![[Screenshot 2026-02-23 at 19.02.35.png]]