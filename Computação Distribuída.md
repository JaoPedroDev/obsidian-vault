# Computação Distribuída
Sistemas de computação distribuída, são modelos projetados com o objetivo de compartilhar recursos, desempenho, confiabilidade, tolerância a falhas e escalabilidade.

## Computação em Cluster
É um modelo de computação distribuída de alto desemepnho, necessita do mesmo OS em todos os computadores, hardware semalhante e uma rede local de alta velocidade.

É formado por um computadore mestre, responsável por controlar, enviar tarefas e balancear a carga dos computadores escravos.

Para seu uso efetivo, a aplicação deve ser feita especificamente para rodar em um cluster, dividindo as tarefas entre os computadores.

## Computação em Grade (Grid Computing)
É um modelo de computação distribuída de alto desempenho, que propõe a configuração de organizações virtuais (OV), em que cada OV contém um grupo de servidores dedicados para executar tarefas da localidade em questão.

Com isso problemas de latência são reduzidos, pois haverá vários servidores distribuídos pelo mundo, ao invés de um único servidor.

## Computação em Nuvem (Cloud Computing)
É um modelo de arquitetura distribuída que oferece um ambiente de serviços de infraestrutura e de sistemas computacionais através da internet.

A estrutura de serviços em nuvem foi dividida em três camadas que atendem a diversos usuários e empresas da seguinte maneira:
- **Software as a Service (SaaS) - Software como um Serviço**: Camada de software que oferece aplicativos como webmail, aplicativos de áudio, vídeo e armazenamento de dados.
- **Plataform as a Service (PaaS) - Plataforma como um Serviço**: Camada para o ambiete de desenvolvimento de sitemas. Possui frameworks para desenvolvimento de software e sistemas gerenciadores de banco de dados.
- **Infraetructure as a Service (IaaS) - Infraestrutura como um Serviço**: Camada para a virtualização de hardware, sistemas operacionais, relatórios gerenciais e dispositivos de armazenamento de dados (storages).

Veja também: [[Segurança de Dados na Nuvem]]

## Arquitetura Orientada a Serviços (Service-oriented Architecture - SOA)
Apresenta uma proposta de interoperabilidade e acoplamento fraco de serviços. Estes serviços podem ser entendidos como um ou mais métodos disponíveis ou um processo grande em execução. Estes serviços são unidades básicas e fundamentais para o desenvolvimento de software. Utilizam padrões e protocolos de comunicação abertos, como, por exemplo, o HyperText Transfer Protocol (HTTP).

## Sistemas de Informação Distribuída
Modelos computacionais que envolvem um conjunto de aplicações e bancos de dados que compõem os sitemas de informação empresarial.

###  Sistemas de Processamento de Transações
Quando um computador cliente submete suas requisições de tranasações a vários seridores ou nós diferentes na rede. Existem dois modelos transacionais;
- Transação Plana: Cliente faz a solicitação da transação para dois ou mais servidores. Só é concluida quando todas as suas requisições são atendidas.
- Transação Aninhada: As transações são executadas paralelamente, pois cada transação pode abrir uma subtransação, e a mesma pode abrir outra subtransação, assim cada transação pode ser executada em servidores diferentes.

Estas transações distribuídas são invocadas através de Chamada de Procedimentos Remotos ou Remote Procedure Calls (RPC).

Soluções ou produtos para o desenvolvimento de transações idstribuídas:
- DCOM (Distributed Compoent Object Model): Solução para RPC de desenvolvimento de aplicações distribuídas, da Microsoft. Substituída pelo .NET.
- CORBA (Common Object Request Broker Architecture): Solução para RPC da OMG (Object Managment Group). Permite que um objeto CORBA possa ser invocado por um outro computador. Este objeto remoto, pode invocar outro objeto em execução em outro computador.
- RMI (Remote Methid  Invocation): Solução Java para RPC. Utiliza a Java Virtual Machine (JVM).
- WS (Web services): Solução utilizada em RPCs que podem se conectar a internet. Utiliza o protocolo SOAP (Simple Object Access Protocol) que empacota as mensagens XML) para comunicação. Assim criando uma independência de linguagem de programação.

### Middleware de Aplicações Corporativas
É uma solução que causa a coesão ou integração do sistema. Assim, muitas aplicações antigas e desenvolvidas para um propósito único (conhecidas também por sistemas legados), que não possuem interoperabilidade alguma e dificultam o acesso as informações por elas mantidas. O modelo de _Middleware_ permite criar uma camada intermediária entre as aplicações distribuídas ou não, onde serviços podem ser executados viabilizando a coesão do sistema.

## Sistemas Distribuídos Pervasivos
Modelos que envolvem dispositivos móveis e ubíquos e, que de maneira geral, estão associados ao avanço tecnológico para a redução de tamanho (miniaturização) e a conectividade com as redes sem fio.

## Computação Ubíqua
A computação ubíqua representa "em toda parte", pois os sistemas computacionais evoluíram de tal maneira que os computadores passaram a fazer parte do cotidiano do homem em qualquer lugar. Estes dispositivos, muitos deles formados por PDAs, computadores, leitores de código de barras, TVs, dispositivos móveis etc, estão presentes no ambiente do usuário que consome estes recursos de conexão e informação.

# Tags
#hardware #computador #arquiteturadecomputação 
# Veja Também
- [[Arquiteturas Paralelas e Taxonomia de Flynn]]
- [[Sistemas de Computação]]
- [[Máquina Virtual]]