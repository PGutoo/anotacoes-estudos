
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

AWS Lambda é um serviço de computação sem servidor que ajuda os usuários a executar códigos sem provisionar nem gerenciar servidores. Você paga apenas pelo tempo de computação consumido. Não há cobrança quando o código não está em execução.

Com o Lambda, você pode executar código para praticamente qualquer tipo de aplicativo ou serviço de back-end, sem precisar de administração. Você só precisa fazer o upload do código e o Lambda gerencia todos os itens necessários para executar e dimensionar o código com alta disponibilidade. Você pode configurar seu código para ser iniciado automaticamente a partir de outros serviços da AWS ou chamá-lo diretamente em qualquer aplicativo web ou para dispositivos móveis.

### Amazon ECS

O Amazon Elastic Container Service (Amazon ECS) é um serviço de gerenciamento de contêineres altamente dimensionável e de alto desempenho. Ele ajuda os clientes a criar novos contêineres e a gerenciá-los nas instâncias do EC2. O Amazon ECS é compatível com contêineres Docker. O Docker é uma plataforma de software que empacota softwares (tais como aplicativos) em contêineres.

Para gerenciar seus contêineres, você deve instalar um agente de contêiner de código aberto do Amazon ECS em suas instâncias do EC2. Esse agente é chamado de instância de contêiner. Você pode executar esse agente em Linux, Windows e Amazon Machine Images (AMIs). O Amazon ECS usa chamadas de API para controlar aplicativos habilitados para Docker.
### Amazon EKS

O Amazon Elastic Kubernetes Service (Amazon EKS) oferece flexibilidade para iniciar, executar e dimensionar aplicativos Kubernetes na Nuvem AWS ou on-premises (no local). Kubernetes é uma plataforma de código aberto para gerenciamento de aplicativos em contêiner. Ele é portátil e extensível.

Com o Amazon EKS você poderá fornecer clusters seguros e de alta disponibilidade. Ele automatiza a aplicação de patches, provisionamento de nós, e atualizações.
### AWS Fargate

O AWS Fargate é um mecanismo de computação sem servidor para contêineres. Ele oferece suporte às arquiteturas Amazon CcS e Amazon EKS. O Fargate aloca a quantidade certa de computação, reduzindo a necessidade de gerenciar instâncias do EC2, capacidade de cluster e scaling.

### AWS Elastic Beanstalk

O AWS Elastic Beanstalk é um serviço de fácil utilização para implementação e scaling de serviços e aplicativos da web. Você pode fazer o upload do seu código que o Elastic Beanstalk se encarrega automaticamente da implantação, desde provisionamento de capacidade, balanceamento de carga e auto scaling até o monitoramento da integridade do aplicativo. Ao mesmo tempo você mantém total controle sobre os recursos da AWS que possibilitam a operação do seu aplicativo, e pode acessar os recursos subjacentes a qualquer momento.

Não há cobrança adicional pelo Elastic Beanstalk. Você paga apenas pelos recursos da AWS necessários para armazenar e executar seus aplicativos.


# Introdução ao Amazon EC2

## Tipos de instâncias

Os tipos de instâncias apresentam várias combinações de CPU, memória, armazenamento e capacidade de rede. Essa variedade proporciona flexibilidade para escolher a combinação apropriada de recursos para seus aplicativos.
Podendo ser usadas para em específico, aplicações ou memórias otimizadas para Big Data e caches e instâncias baseadas em gráfico para machine learning.

## Scaling

Com auto scaling é possível escalar uma instância para cima ou para baixo, atendendo rapidamente a mudanças nos requisitos. Ajuda a reduzir o foco no tráfego, para que tenha foco em desenvolvimento.
Essa escalabilidade existe pois a AWS permite posicionar instâncias em diversas Zonas de Disponibilidade. Cada região do Amazon EC2 tem 99,99% de garantia de inatividade quase zero.

## Econômico

É possível otimizar os custos com base nas necessidade e pagar apenas o que utilizar. É possível criar e destruir instâncias e pagar apenas pelo eventual armazenamento de dados que decidir não excluir.
Existem opções de custo:

- On-Demand Instances - Paga conforme o uso
- Saving Plans - Preços mais baixos por um compromisso de 1 a 3 anos
- Dedicated hosts - Servidores físicos dedicados
- Spor instances - Para aplicativos com horários de início e término flexíveis.

## Provisionamento

Ao provisionar você decide:

- Sistema operacional
- Detalhes de rede
- Opções de armazenamento
- Configurações de segurança

# Que problemas o Amazon EC2 resolve?

## Execução de servidores on-premises

- Necessidade de prever aumentos súbitos de tráfego e picos nas cargas de trabalho.
- Necessidade de considerar a possibilidade de servidores não utilizados ou ociosos.
- Custo de recursos não utilizados.

## Execução de servidores no Amazon EC2

- Não é preciso adivinhar a capacidade.
- Inicie servidores quando precisar deles.
- Encerre ou interrompa instâncias quando não precisar mais delas.
- Pague somente pelo que usar.

# Visão geral do Amazon EC2

- O Amazon EC2 pode hospedar os mesmos tipos de aplicativos que você executaria em um servidor tradicional local. Ele disponibiliza capacidade computacional segura e redimensionável na nuvem.
- Fornece máquinas virtuais, chamadas de instâncias do EC2, na nuvem.
- Oferece controle total sobre o sistema operacional convidado (Windows ou Linux) de cada instância.
- É possível iniciar instâncias de qualquer tamanho em uma Zona de Disponibilidade em qualquer lugar do mundo.
	- Inicie instâncias com apenas alguns cliques ou uma linha de código e elas estarão prontas em minutos.
- Você pode controlar o tráfego de entrada e saída das instâncias usando:
	- Grupos de segurança
	- Elastic Load Balancing (ELB)

Usos comuns das instâncias EC2 incluem servidores de aplicativos:
- Servidores WEB
- Servidores de banco de dados
- Servidores de jogos
- Servidores de e-mail
- Servidores de mídia
- Servidores de catálogo
- Servidores de arquivos
- Servidores de computação
- Servidores de proxy

# Benefícios do Amazon EC2

## Computação elástica

Você pode usar o Amazon EC2 para aumentar ou diminuir a capacidade computacional em minutos, em vez de horas ou dias. É possível contratar simultaneamente uma, centenas ou até milhares de instâncias de servidor. Você também pode usar o Auto Scaling do Amazon EC2 para manter a disponibilidade de sua frota do Amazon EC2, e dimensionar sua frota para cima e para baixo automaticamente, dependendo de suas necessidades, para maximizar o desempenho e minimizar os custos. Para dimensionar vários serviços, você pode usar o Auto Scaling da AWS.

## Controle completo

Você tem controle completo das suas instâncias, incluindo acesso-raiz, bem como a possibilidade de interagir com elas como faria com qualquer computador. Você interromper qualquer instância enquanto retém os dados na partição de inicialização e, em seguida, reiniciar a mesma instância usando APIs de serviço da web. As instâncias podem ser reinicializadas remotamente usando APIs de serviço da Web, e você também tem acesso à saída do console.

## Serviços de hospedagem flexíveis

Você pode escolher vários tipos de instâncias, sistemas operacionais e pacotes de software. Com o Amazon EC2, você pode selecionar uma configuração de memória, CPU, armazenamento de instâncias e tamanho da partição de inicialização ideal para seu sistema operacional e aplicativo. Por exemplo, os sistemas operacionais disponíveis incluem várias distribuições do Linux e o Microsoft Windows Server.

## Integrado

O Amazon EC2 é integrado à maioria dos serviços da AWS. Esses serviços podem incluir o Amazon Simple Storage Service (Amazon S3), o Amazon Relational Database Service (Amazon RDS) e o Amazon Virtual Private Cloud (Amazon VPC), por exemplo. Essa integração fornece uma solução completa e segura para computação, processamento de consultas e armazenamento na nuvem por meio de uma ampla variedade de aplicativos.

## Confiável

O Amazon EC2 fornece um ambiente altamente confiável no qual a substituição de instâncias pode ser rápida e previamente encomendada. O serviço é executado dentro dos data centers e da infraestrutura de rede comprovada da Amazon.

## Seguro

Segurança é a maior prioridade da AWS. Como cliente da AWS, você se beneficiará de um data center e uma arquitetura de rede construídos para atender a organizações com os mais rigorosos requisitos de segurança. O Amazon EC2 funciona em conjunto com a Amazon VPC para oferecer funcionalidades de rede seguras e robustas para seus recursos de computação.

## De baixo custo

Usando o Amazon EC2, você pode aproveitar a escala da Amazon, pagando uma taxa muito baixa pela capacidade de computação que você realmente consome.

## Comece a usar rapidamente

Você pode começar a usar o Amazon EC2 rapidamente Seja iniciando uma instância programaticamente ou por meio do console de gerenciamento da AWS, suas instâncias estarão prontas para uso em minutos. Quando não precisar mais das instâncias, você poderá interrompê-las ou encerrá-las tão rápido quanto as iniciou.

# Arquitetura do Amazon EC2

Você decide qual região, nuvem privada virtual (VPC), sub-rede e grupo de segurança deverá colocá-la.

A AWS tem regiões em todo o mundo, elas são a parte externa da arquitetura, em seguida escolhe qual VPC da AWS deseja colocar usa instância do EC2. Em cada VPC, você pode especificar a sub-rede, cada instância do EC2 será colocada por trás de um grupo de segurança, com as configurações de segurança que você definiu ao iniciar a instância.
Para alta disponibilidade, uma prática recomendada é colocar suas instâncias em várias sub-redes em diferentes Zonas de Disponibilidade. Em seguida, tenha um Elastic Load Balancer anexado para rotear o tráfego com base nas necessidades do aplicativo.

![[Pasted image 20250328154609.png]]

# Casos de uso do Amazon EC2

- Executar aplicativos empresariais e nativos na nuvem - O Amazon EC2 oferece infraestrutura de computação segura, confiável, de alto desempenho e econômica, para atender às necessidades exigentes dos negócios.
- Dimensionar para aplicativos de computação de alto desempenho (HPC) - Acessar a infraestrutura e a capacidade sob demanda de que você precisa para executar aplicativos HPC com mais rapidez e melhor custo-benefício.
- Desenvolver para plataformas da Apple - Construir, testar assinar cargas de trabalho sob demanda para MacOS. Acessar ambientes em minutos, dimensionar dinamicamente a capacidade quando necessário, e se beneficiar do pagamento conforme o uso da AWS.
- Treinar e implantar aplicativos de machine learning (ML) - O Amazon EC2 oferece a mais ampla variedade de serviços de comutação, rede (até 400 Gbps) e armazenamento, desenvolvidos especificamente para otimizar o desempenho e preço em projetos de ML.

# Custo de instâncias

5 principais fatores que afetam o custo da instância:

- Opções de compra de instâncias
- Tenancy
- Amazon Machine Image (AMI)
- Tipos de instância do EC2
- Tipo e tamanho do armazenamento
## Opções de compra de instâncias

Ao escolher uma opção de compra de instância, você deve considerar o seguinte:
- O caso de uso da instância
- A estrutura de custos da opção de compra

### Instâncias sob demanda

- Pague por capacidade computacional por segundo (para Amazon Linux e Ubuntu)
- Não há compromissos de longo prazo
- Não há pagamentos antecipados
- Aumente ou diminua a capacidade computacional dependendo das demandas de seu aplicativo


| Caso de uso                                                   | Problema solucionado                             |
| ------------------------------------------------------------- | ------------------------------------------------ |
| Cargas de trabalho de curto prazo, com picos ou imprevisíveis | Atende à necessidade de capacidade computacional |
| Desenvolvimento ou teste de aplicativos                       |                                                  |

### Instâncias reservadas

As instâncias reservadas podem oferecer um desconto significativo para suas arquiteturas.
- Até 72% de desconto em comparação com as instâncias sob demanda
- Pagamento antecipado por capacidade (opções de compra de 1 ou 3 anos)
- Três métodos de pagamento antecipado:
	- IRs padrão
	- IRs conversíveis
	- IRs programadas


| Caso de uso                                                                                           | Problema solucionado                                              |
| ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| Cargas de trabalho previsíveis, que não exigem flexibilidade de poder computacional                   | Possibilita reservar capacidade antecipadamente, reduzindo custos |
| Cargas de trabalho com duração maior que 1 ano                                                        |                                                                   |
| Os usuários podem fazer pagamentos antecipados, reduzindo ainda mais o total dos custos de computação |                                                                   |

### Instâncias de Savings Plans

A AWS oferece dois tipos de Saving Plans:
- Os *Compute Saving Plans* fornecem maior flexibilidade e ajudam a reduzir seus custos em até 66%.
	- Esses planos se aplicam automaticamente ao uso de sua instância do EC2, independentemente da família da instância, tamanho, Zona de Disponibilidade, Região, sistema operacional ou tenancy. Também são aplicáveis ao uso do AWS Fargate e do AWS Lambda.
- Os *EC2 Instace Savings Plans* se aplicam a uma família de instâncias específica em uma Região específica, e oferecem o maior desconto (até 72%, como as IRs padrão)


| Caso de uso                                                                                                | Problema solucionado                     |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Cargas de trabalho de longo prazo                                                                          | Não precisa coordenar suas comprar de IR |
| Necessidades de computação que possam demandar mais flexibilidade do que localização ou poder de instância |                                          |

### Instâncias spot

- Compre capacidade não utilizada do Amazon EC2
- Até 90% de desconto em comparação com o preço sob demanda
- Preços controlados pela AWS com base em oferta e demanda
- Aviso de encerramento 2 minutos antes de encerrar
- Blocos spot: Inicie instâncias spot com duração de 1 a 6 horas


| Caso de uso                                                                                            | Problema solucionado                                                                                                                  |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------- |
| Aplicativos com horários de início e término flexíveis                                                 | Cargas de trabalho de baixo orçamento podem ser atendidas com instâncias de baixo custo, desde que se tenha tolerância a interrupções |
| Aplicativos que só serão viáveis se tiverem preços de computação muito baixos.                         |                                                                                                                                       |
| Usuários com necessidades computacionais urgentes que exijam grande quantidade de capacidade adicional |                                                                                                                                       |
