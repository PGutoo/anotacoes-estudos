
Computação é o cérebro por trás dos aplicativos de T.I
Dependendo da carga de trabalho, você pode precisar de um método arquitetônico diferente para o modo como você configura os recursos computacionais.

## O que é computação?

Computação é o cérebro que faz os aplicativos de TI funcionarem, coleta todos os dados necessários, analisa, processa e finalmente distribui.
Componentes principais:

- **CPU**: Executa e processa as instruções que recebe.
- **RAM**: Armazena dados que o computador precisa para realizar tarefas de processamento. Armazenamento temporário.
- **Disco Rígido**: Armazenamento de longo prazo. Armazena os arquivos de inicialização e arquivos criados por você.
- **Desempenho de rede**: *Largura de banda* - Quantidade de dados que podem ser enviados ao longo de um determinado período. *Latência* - O tempo que leva para os dados serem transportados.

Todos computadores tem um sistema operacional que serve para gerenciar o hardware e o software do computador. Exemplo: Windows, Linux e MacOs.

Com as tecnologias de virtualização surgiram nuvens, um serviço sob demanda para recursos de computação e TI pela internet, com pagamento conforme o uso.
Benefícios:

- **Economia de custos**: Não há custos iniciais. Pague somente pelo que usar. Nenhum data center para manter
- **Dimensionável**: Aumenta e reduz verticalmente conforme a necessidade. Não é preciso adivinhar a capacidade. Provisiona recursos conforme o necessário.
- **Confiável**: Serviços confiáveis. Construído pensando em tolerância a falhas. Integridade do aplicativo.

## Métodos de computação

### Instâncias

**Uma instância**, ou máquina virtual, é um recurso de computação na nuvem. A instância funciona como um servidor local tradicional. Ela pode dar suporte a cargas de trabalho como hospedagem na web, aplicativos, bancos de dados, serviços de autenticação, e tudo que um servidor pode fazer. Você escolhe o sistema operacional (OS), a CPU, a memória, o armazenamento, e outros componentes, e em alguns minutos sua instância está pronta para uso. Ao terminar sua tarefa, você pode interromper ou encerrar as instâncias. Você não fica preso a servidores que não quer, ou dos quais não precisa. Você pode tratar as instâncias como recursos de computação temporários e descartáveis, livres da inflexibilidade e das restrições de uma infraestrutura de TI fixa e finita.

#### **Casos de uso de instâncias** incluem:

- Ambiente de hospedagem
- Ambientes de desenvolvimento e teste
- Backup e recuperação de desastres

### Contêineres

Os **contêineres** são um método de virtualização do sistema operacional que você pode usar para executar um aplicativo e suas dependências em processos isolados de recursos. Ao usar contêineres, você pode empacotar o código, as configurações e as dependências de um aplicativo em blocos de construção simples, garantindo consistência ambiental, eficiência operacional, produtividade do desenvolvedor e controle de versão.

Os contêineres são menores que as máquinas virtuais e não contêm um sistema operacional completo. Em vez disso, eles compartilham um sistema operacional virtualizado e são executados como processos isolados de recurso, o que garante implantações rápidas, confiáveis e consistentes. Os contêineres têm tudo que o software precisa para ser executado, como bibliotecas, ferramentas do sistema, código e runtime.

#### **Casos de uso de contêineres** incluem:

- Construção de arquitetura de microsserviços
- Serviços de renderização de vídeo
- Desenvolvimento e implantação rápidos

### Serveless

A **computação sem servidor** possibilita que você execute código sem provisionar ou gerenciar servidores. A computação sem servidor apresenta auto scaling, alta disponibilidade integrada e um modelo de cobrança conforme o uso, para aumentar sua agilidade e otimizar seus custos. A computação sem servidor também elimina tarefas de gerenciamento de infraestrutura, como provisionamento de capacidade e aplicação de patches, para que você possa se concentrar em escrever códigos que sirvam seus clientes.

#### **Casos de uso de sem servidor** incluem:

- Processamento de arquivos
- Aplicativos web
- Back-end para dispositivos móveis
- Cron jobs (tarefas de computação agendadas)

### Híbrida

Em uma implantação híbrida, os recursos baseados na nuvem são conectados à infraestrutura local. Essa abordagem é ideal em várias situações. Por exemplo, se você tem aplicativos legados que são mais bem mantidos no local, ou se as regras governamentais exigem que sua empresa mantenha determinados registros no local.

Suponha que uma empresa queira usar serviços e nuvem capazes de automatizar o processamento de dados e a analytics. No entanto, a empresa tem vários aplicativos legados que são mais adequados à manutenção no local e que não serão migrados para a nuvem. Com uma implantação híbrida, a empresa conseguiria manter os aplicativos legados no local enquanto se beneficiaria dos serviços de dados e analytics executados na nuvem.

#### **Casos de uso híbrido** incluem:

- Aplicativos legados
- Requisitos regulatórios da empresa
- Requisitos regulatórios do governo

## Serviços computacionais da AWS

### Amazon EC2

O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço da web que oferece capacidade computacional segura e redimensionável na nuvem. Você pode usá-lo para provisionar servidores virtuais, chamados de instâncias do Amazon EC2, que podem atender a quase todas as necessidades de computação.

Com o Amazon EC2, você pode:
- Provisionar e iniciar uma ou mais instâncias do EC2 em minutos
- Parar ou encerrar as instâncias do EC2 quando terminar de executar a carga de trabalho.
- Pagar apenas pelo tempo de computação que você usa ao executar uma instância.

### AWS Lambda

- Amazon ECS
- Amazon EKS
- AWS Fargate
- AWS Elastic Beanstalk