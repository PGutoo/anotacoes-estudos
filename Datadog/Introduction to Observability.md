
# Monitoring vs. Observability

## O que é monitoração?

Monitoração é o processo de reunir dados para entender o que está acontecendo dentro da infraestrutura.

## O que é observabilidade?

Observabilidade é obter os mesmos dados coletados e mover para além do "o que está acontecendo?" para "Por que está acontecendo?"

## Três pilares de observabilidade

- Metrics - Esses dados são valores numéricos que podem rastrear qualquer coisa sobre seu ambiente ao longo do tempo.
- Logs - Coleção de informação sobre o uso de uma sistema ao longo do tempo. Um arquivo gerado pelo computador pode conter informações temporais sobre o uso do sistema.
- Traces - Nós dá um entendimento sobre o que está acontecendo dentro de uma aplicação. Usado para rastrear o tempo gasto por uma aplicação processando uma requisição e o status da requisição.

## O que é Metric?

Esses dados são valores numéricos que podem rastrear qualquer coisa sobre seu ambiente ao longo do tempo, de latência até taxas de erros para inscrição de usuários.

### Por que coletamos métricas?

- Linha de base para operações - Métricas podem indicar o que é normal para nossas aplicações. Sem métricas ficamos presos, tentando adivinhar o que está acontecendo.
- Respostas reativas - Usando métricas não temos que esperar até o reporte do usuário. Podemos reagir aos problemas no ambiente antes de uma bola de neve.
- Respostas pro ativas - Por que esperar por algo para dar errado? Olhando as métricas podemos estar a frente do problema antes de acontecer.

### Por que isso importa?

- Resolver problemas antes de estourarem.
- Menos gasto financeiro.
- Menos "incêndios"
- Clientes felizes
- Facilitação do trabalho


## O que é monitoração?

É o ato de analisar padrões que as métricas estão lhe mostrando. É sobre analisar dados e agir com isso.

### O que monitoramos?

- Performance - Analisando a performance podemos observar como nossa arquitetura e aplicações estão utilizando os recursos disponíveis.
- Segurança - Se há algo de errado com o ambiente, criar monitores sobre métricas de segurança pode impedir incidentes.
- Uso - O que os usuários estão fazendo no ambiente? estão interagindo com o produto?

### Quem alertamos?

Alertas - São limites setados em um monitor, quando o limite é estourado uma notificação é enviada para um determinado lugar ou alguém.

Muitos alertas podem ser desgastantes e desnecessários, alertas devem ser muito emergenciais, nem tudo é assim.

## Logs

### O que são logs?

É um arquivo gerado contendo informações sobre o uso do sistema, isso lhe permite ter insight sobre o comportamento dos recursos.

### Por que coletamos logs?

- Conformidade - Os padrões de negócio podem ditar quais logs você precisa armazenar e por quanto tempo.
- Insight - Logs podem fornecer visões do sistema e aplicações que as métricas por si só não conseguem fornecer.
- Segurança - Necessário saber exatamente o que está acontecendo no sistema, dando prioridade ao funcionamento de negócios.

### Usos práticos de logs

- Troubleshooting
- Auditar
- Monitoração
- Alertas

## O que é Trace?

É usado para rastrear o tempo gasto por uma aplicação processando uma requisição ao longo do caminho de execução tomado.

### Span

Porção do todo. Uma unidade do trabalho do que o código está fazendo. (Trace é todos os spans)

### Por que coletamos traces?

- Microsserviços - Em uma arquitetura de microsserviços, possuir o trace de todos os processos se torna essencial.
- Otimização - Permite identificar lentidão que podem ter performance aumentada.
- Troubleshooting - O trace dá suporte para identificar o que há de errado e como corrigir.