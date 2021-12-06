# Máquina Virtual
É um software que faz a emulação de um determinado hardware, possibilitando que um outro sistema operacional seja executado dentro de outro sistema operacional.

## Monitor de Máquina Virtual
Software responsável por hospedar as máquinas virtuais. Ele virtualiza e controla os recursos compartilhados pelas máquinas viruais. Também escalona qual VM vai ser executada a cada momento.

O monitor de VM é dividido em duas categorias de acordo com seu acesso ao hardware:
- **Baremetal**: Roda diretamente no hardware do servidor. Monitora os OS convidados, controla e compartilha os recursos do hardware. Ele proporciona:
	- Segurança sobre os recursos virtualizados
	- Agilidade de reconfigurar recursos computacionais.
- **Hosted**: Executado dentro de um OS hospedeiro e não tem acesso direto ao hardware.

## Virtualização
É um estrutura ou metodologia que divide os recursos de uma plataforma fisica de computador em múltiplos ambientes de execução. Atualmente a linguagem mais usada para os softwares de virtualização é o Java.

### Técnicas de virtualização
Há duas técnicas básicas:
- **Virtualização Total**: Fornece ao OS convidado uma réplica do hardware subjacente. Assim ele é executado sem modificações. Utiliza um grande conjunto de dispositivos genéricos fornecido ao monitor de máquina virtual. Algumas das vantagens:
	- Isolamento completo de cada VM
	- OS são instalados sem nenhuma modificação
	- Suporta performance de processador e memória
	- Técnicas sofisticadas para interceptar e emular instruções.
- **Paravirtualização**: O OS convidado e o monitor de máquina virtual se comunicam. Vantagens:
	- OS modificado para chamar p monitor de VM sempre que executar uma instrução sensível, acabando com a necessidade de o monitor de VM testar instrução por instrução.
	- Os dispositivos de hardware são acessados por drivers da própria máquina virtual.

# Tags

# Veja Também
- 