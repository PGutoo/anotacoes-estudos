
# Virtualização

## Como funciona?

A virtualização surgiu como uma forma de separar o melhor do hardware do software. No modelo tradicional, os softwares são instalados em um sistema operacional, que por sua vez, está instalado sobre uma infraestrutura física (o hardware). Contudo, sempre que a demanda de software aumenta, a infraestrutura física precisa ser substituída por outra mais poderosa (processadores mais rápidos, mais memória, etc), isso é chamado de upgrade vertical. O upgrade horizontal é definido pelo aumento de computadores para atender uma demanda maior, nesse modelo, cada computador tem sua própria estrutura de sistema operacional, portanto, seus próprios processos.

A virtualização possibilitou a abstração do hardware, pois uma camada de software mimetizando uma infraestrutura física é inserida entre o hardware (real) o sistema operacional, possibilitando uma separação mais eficiente destas duas camadas. A virtualização permite, por exemplo, a instalação de vários sistemas operacionais em um mesmo equipamento.

O inverso surgiu logo depois, um único sistema operacional instalado sob uma única camada de virtualização que compreende diversos computadores abaixo dela. Essa máquina virtual "enxerga" um único hardware, permitindo uma flexibilidade muito grande no aumento destes recursos para a máquina virtual. Sempre que esta precisar atender mais usuários, poderá receber rapidamente mais processamento e memória e, por sua vez, sempre que a infraestrutura física for insuficiente, novos computadores serão adicionados ao cluster em um upgrade horizontal.

## Benefícios

Esta tecnologia permite simular aplicações, servidores, armazenamento e redes, sendo capaz de reduzir custos, aumentar eficiência, agilidade, flexibilidade e escalabilidade dentro de uma infraestrutura corporativa.

Com a virtualização é possível consolidar servidores, cargas de trabalho e ambientes, aumentar a utilização de recursos e acelerar a implantação de desktop e aplicativos.

- **Redução de custos**: A virtualização pode reduzir investimentos em hardware, energia e espaço físico, isso porque permite reaproveita recursos físicos que ficam ociosos.
- **Redução do tamanho do parque de equipamentos (datacenter)**: Com o melhor aproveitamento dos recursos atuais, a necessidade de aquisição de novos equipamentos diminui, reduzindo gastos com instalação, refrigeração, espaço físico, manutenção, consumo de energia e assim por diante.
- **Gerenciamento centralizado**: Torna-se mais fácil monitorar serviços/processos em execução, já que o gerenciamento destes é feito de forma centralizada (no entanto, isso depende da estratégia de virtualização adotada).
- **Manutenção de sistemas legados**: Um grande desafio nas grandes empresas é. sem dúvida alguma, a manutenção de sistemas legados. Não é raro encontrar um equipamento cujo *hardware* possui mais de vinte anos de idade, rodando um sistema operacional absolutamente obsoleto com o único objeto de manter "no ar" uma aplicação ou serviço que "só roda naquela configuração específica". A virtualização permite simular aquele *hardware* que já deveria ter sido aposentado há muito tempo.
- **Ambientes de testes**: A virtualização permite até mesmo emular hardwares de arquiteturas diferentes. Como testar uma aplicação feita para funcionar em um *smartphone* Android ou um Iphone? Claro que você pode comprar os equipamentos, mas nem sempre é uma opção: um desenvolvedor de aplicativos preocupado com seus usuários teria que possuir vinte *smartphones* diferentes (chutando baixo). Por meio da virtualização, é possível simular um arquitetura ARM (advanced RISC Machine), típica de *smartphones*, em um arquitetura x86-64 bits (dos microcomputadores).
- **Confiabilidade e Segurança**: Já que cada máquina virtual (VM) funciona de maneira independente, se um problema surgir em uma delas (como uma vulnerabilidade de segurança, por exemplo) este não afetará as demais.
- **Migrações e ampliações mais simples**: Trocar um fornecedor da infraestrutura *Cloud Computing* é mais simples, pois a VM pode ser exportada e importada em outro ambiente com facilidade (a alterativa seria montar o sistema todo de novo, "do zero"). Além disso, ampliar o hardware demandando mais processamento, memória ou armazenamento se torna mais flexível, graças ao compartilhamento de *hardware* e *upgrades* horizontais.

# Por dentro da Máquina Virtual

## Infraestrutura


Pode-se dizer que uma Máquina Virtual (ou Virtual Machine, VM), nada mais é que um computador emulado, que possui processador, memória, armazenamento, rede, interfaces (como a USB) e até periféricos emulados, com a capacidade de executar as mesmas funções que um computador físico.

## Hardware

Esse é o um dos principais itens dentro da tecnologia de virtualização, um sistema operacional pode ser instalado sobre outro tipo de sistema, com seus recursos de hardware sendo representados via software

## Armazenamento

Também conhecido pelo nome de **Software Defined Storage - SDS - (Armazenamento Definido por Software)**. É uma camada de software criada sobre discos físicos, onde os dispositivos acessam discos, de modo a tornar o acesso mais flexível, gerenciável e personalizável.

## Rede

Chamado de **Software Defined Networking - SND (Rede Definida por Software)**. É possível criar um tipo de infraestrutura lófica (software) de redes sobre uma determinada rede física, permite a configuração e o detalhamento de acordo com as necessidade do ambiente.