A blockchain fornece registros digitais do tipo "quem possui o quê?".
- Sem autoridade central, sem armazenamento central
- Mecanismos para garantir a escalabilidade, integridade e confiança
#### **4 Pilares da blockchain:**
1.  **Descentralizada** - Sem autoridade central.
2.  **Distribuída** - Cada nó possui uma cópia na blockchain.
3.  **Imutável** - Uma vez adicionado um bloco, ele não pode ser alterado ou removido.
4.  **Confiável** - Participantes confiam no sistema, e não em outros participantes.
#### **Blocos e transações**
Cada bloco contém:
1. Conjunto de transações
2. Hash do block anterior
3. Timestamp (quando a ação foi feita)
4. Hash das transações
5. Prova associada ao mecanismo de consenso
#### **Mecanismos de consenso**
São estes mecanismos que garantem que todos os nós concordem sobre o estado da blockchain:
1. **Proof of Work (PoW)** - Poder computacional decide quem cria o bloco (alto consumo energético - Bitcoin)
2. **Proof of Stake (PoS)** - Participação (riqueza/stake) define validadores (Ethereum)
3. **Proof of Authority (PoA)** - Validadores pré-selecionados (mais centralizado)

### **Tipos de Blockchain**
- **Pública sem permissão**: qualquer um pode ler e escrever (Bitcoin, Ethereum).
- **Pública com permissão**: leitura restrita, escrita aberta.
- **Privada sem permissão**: leitura aberta, escrita restrita.
- **Privada com permissão**: leitura e escrita restritas (mais próxima de um banco de dados distribuído).

![[Screenshot 2026-01-08 at 14.42.50.png]]

#### **Smart Contracts**
São programas executados na blockchain que definem regras e ações automáticas, imutáveis e verificáveis, executadas quando determinadas condições são atendidas.
Eles funcionam como:
- **Regras de negócio on-chain**
- **Contratos digitais autoexecutáveis**
- **Mecanismos de automação confiável sem intermediários**

**Na prática:**
1. Um contrato é escrito em código
2. Implantado na blockchain
3. Seu código torna-se:
	- Público (ou visível aos participantes, em permissionadas)
	- Imutável
4. Sempre que é chamada:
	- Executa exatamente a mesma lógica para qualquer nó
5. O resultado é: 
	- Consensual
	- Auditável
	- Não repudiável