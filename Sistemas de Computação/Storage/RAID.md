# RAID
RAID é a técnica de combinar múltiplos disk drives em uma unidade lógica (RAID Set) e ainda promover proteção, performance, ou os dois.

## Métodos de implementação RAID
Existem dois métodos de implemtação de RAID, RAID em software e RAID em hardware.
### RAID em software
Utiliza o software do host para prover as funcionalidas. Sendo implementado a nivel do OS. É o modelo mais barato, porém possui mais limitações:
- Performance: Afeta a performance do sistema como um todo e ainda requer a efetuação de cálculos de RAID na CPU.
- Funcionalidades: Não suporta todas os niveis de RAID
- Compatibilidade com o OS: RAID em software é uma fatia do OS, portanto upgrades para o software RAID ou OS tem que ser valido para ambos.

### RAID em hardware
O controle externo de RAID é um hardware baseado no array do RAID e age como uma interface entre o host e os discos. Ele representa um volume de storage para o host e o host administra estes volumes como se fossem discos físicos. As funções chaves do controlador RAID são:
- Administrar e controlar agregações de discos
- Transcrever as requisições de I/O enre discos lógicos e físicos
- Regeneração de dados em uma eventual falha do disco

## Componentes do Array RAID
Um array RAID é um compartimento que abriga um conjunto de drives de disco qeu ajudam o hardware a implementar o RAID.

## Técnicas RAID
Existem três técnicas usadas pra RAID.
### Striping
Striping é a técnica de espalhar os dados através de vários disk drives (mais de um) com o objetivo de utilizar os drives em paralelo. Assim, mais dados são processados ao mesmo tempo, aumentando a performance do sistema.

Dentro de cada disco do RAID são definidos um número de blocos endereçáveis con´tiguos como uma tira(stripe).

O stripe size decreve o número de blocos em uma faixa e é o número máximo de dados que podem ser escritos ou lidos a partir de um único disco no conjunto antes que o próximo disco seja acessado, assumindo que o dado se inicia no começo da faixa. O dado é quebrado em pequnas partes quando espalhado pelo disco.

### Mirroring
Técnica onde o mesmo dado é gravado em dois ou mais disk drivers diferentes. Ela é usada para garantir a segurança dos dados, pois se um disk driver falhar haverá uma cópia de todos os dados no outro hd.

É considerado um recurso caro, portanto é utilizada apenas em aplicações que requerem uma segurandça adicional.

### Parity
Um disk drive adicional é adicionado ao conjunto stripe com a finalidade de armazenar a paridade e um calculo matemático permite a recriação do dado perdido. Parity é uma técnica de redundância que assegura a proteção do dado sem que seja necessário a manutenção de um conjunto completo do dado em duplicidade. O calculo da paridade é uma função do controlador RAID.

## Recuperação de dados na técnica de paridade.
Considerando o exemplo de uma configuração de RAID contendo cinco discos, onde quatro deles guardam dados e o quinto guarda a informação de paridade. Neste caso a paridade necessita apenas de 20 por cento de espaço em disco extra, entretanto a paridade é recalculada a cada mudança no dado. Este recalculo consome tempo e afeta a performance do controlador RAID.

## Níveis de RAID
A performance da aplicação e os requerimentos de disponibilidade dos dados determinam a seleção do nível de RAID.

Esses níveis são definidos com base nas técnicas de striping, mirroring e parity. Alguns níveis de RAID utilizam uma simples técnicas, embora outros utilizam uma combinação de técnicas.

### RAID 0
Utiliza a técnica de data striping. Utiliza toda a capacidade de armazenamento do conjunto de discos do RAID. Para ler o dado, todas as filas são colocadas juntos pelo controlador. Quando o número de drives no conjunto aumenta a performance do conjunto também aumeta em função de mais dados poderem ser lidos ou gravados simultaneamente.

### RAID 1
Utiliza a técnica de espelhamento(mirroring). Consiste de dois disk drivers e tudo é  espelhado nos dois discos.

### RAID 1 + 0 / RAID 10
Combina os RAIDs 1 e 0. Necessita de um número par de drives, sendo o mínimo 4 drives. O elemento básico desse RAID é o espelhamento do par, ou seja, o dado primeiramento é espelhado e depois as duas cópias são fatiadas através de múltiplos discos do conjunto RAID.

### RAID 3
Fatia os dados para alta performance e utiliza a paridade para tolerância a falhas. As informações de paridade são armazenadas em um drive dedicado.

### RAID 5
É uma implementação muito versátil. Ele utiliza o fatiamento. Os drives são acessados de forma idependente. A pariedade é distribuída e gravada por todos os discos evitando o gargalo de gravação no disco de paridade.

### RAID 6
Similar ao RAD5, exceto que existe a inclusão de um segundo elemento de paridade que permite a sobrevivência em um ebento de falha de disco no conunto RAID. RAID 6 distribui a paridade através de todos discos.

# Tags
#hardware #arquiteturadecomputação
# Veja Também
- [[Sistema de Armazenamento (Memórias)]]
- [[Sistemas de Computação]]
- [[Sistemas de Backup]]