# Intelligent Storage System
É um conjunto de funcionalidades do RAID array que contribuem com o funcionamento automatizado e performático do RAID.

## Principais componentes
Consiste de quatro componentes: front end, cache, back end e os discos físicos. Nos modernos equipamentos de hoje em dia, inteligent storage systems, front end, cache e back end, são tipicamente integrados em uma única placa chamada storage processor ou diretor.

### ISS - Front End
Prove a interface entre o storage system e o host. Consiste das portas front end e os controladores do frond end.

Cada controlador do front end possui um processador lógico que executa o protocolo de transporte apropriado, do tipo Fiber Channel, iSCSI, FICON ou FCoE para as conexões do storage o front end controller roteia o dado do e para o cache via barramentos de dados internos. Quando o cache recebe o dado para ser gravado, o controlador envia uma mensagem de "acknowledgmente" para o host.

### ISS - Cache
Usado para aumentar a performance, pois ele armazena os dados recentemente acessados pelo I/O, assim não precisa buscar um dado recente mais de uma vez.

### ISS - Back End
Promove uma interface entre o cache e os discos físicos. Consiste da porta de back end e controlador de back end. Controla a transferência entre o cache e os discos fisicamente.

Para uma alta proteção e disponibilidade de dado, o storage system é configurado com dois controladores e múltiplas portas As configurações provêm um caminho alternativo para os discos físicos em evento de falha em controle ou porta.

### ISS - Discos Físicos
São conectador no back end no controlador do storage e provê um armazenamento de dados persistente. O ISS provê suporte para uma variedade de disk drives com diferentes funcionalidades.

## Tipos de armazenamento ISS: High-end Storage System
High-end storage system se refere a tabelas do tipo ativo - ativo e são geralmente montadas em grandes empresas. Estes sistemas são desenhados com um grande número de controladores e memória cache. Um ativo - ativo array implica que o host pode executar I/Os através dos controladores disponíveis, conforme:
- Grande capacidade de armazenamento.
- Grande quantidade de caches para otimizar os serviço de I/O para o host.
- Arquitetura tolerante a falha para garantir a disponibilidade do dado.
- Conectividade com computadores mainframe e do tipo open system.
- Disponibilidade para múltiplas portas front-end e protocolos de interface para um grande número de host.
- Disponibilidade de múltiplos back-end fiber channel ou controladores de RAID SCSI para administrar os processos de disco.
- Escalabilidade para suportar a crescente solicitação de conectividade, performance e capacidade de storage.
- Habilidade para administrar um grande número de I/Os vindos das aplicações em hosts.
- Suporte para replicação de dados tanto local como remoto.

## Tipos de ISS: Midrange Storage System
Se referem a array ativo - passivo e são melhor alocados em empresas de tamnaho pequeno ou médio. O host pode exectuar I/Os apenas através de controlador que seja dodo do LUN. O host pode executar leituras ou gravações no LUN apenas através do caminho do controlador A, porque o controlador A é dono da LUN. O caminho do controlador B continua passivo e nenhuma atividade I/O é executada.


# Tags
#computador #bancodedados #armazenamento  
# Veja Também
- [[RAID]]
- [[Sistemas de Backup]]
- [[Sistema de Armazenamento (Memórias)]]