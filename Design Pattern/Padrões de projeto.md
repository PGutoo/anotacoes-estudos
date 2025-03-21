
# O que são?

São soluções elegantes para problemas conhecidos recorrentes no desenvolvimento de softwares  que foram utilizados e testados no passado e continuam relevantes nos dias atuais.

São divididos em 3 categorias: de criação (creational), que visam abstrair o processo de como os objetos são criados na aplicação; estruturais (structural), que lidam com a composição de classes e objetos; comportamentais (behavioural), que caracterizam como as classes e objetos interagem e distribuem responsabilidades na aplicação.

# O que é bom?

- Você não precisa reinventar a roda.
- Padrões universais facilitam o entendimento do seu projeto.
- Evita refatoração desnecessária.
- Ajuda na reutilização de código (conceito DRY - Don't repeat yourself).
- Abstrai e nomeia partes particulares do projeto.
- Ajuda na aplicação dos princípios do design orientado a objetos (SOLID).
- Facilitam a criação de testes unitários.

# O que é ruim?

- Alguns padrões podem ser complexos até que você os compreenda.
- Muito código para atingir um objetivo simples.
- Podem trazer otimizações prematuras para seu código (YAGNI - You ain't Gonna need it).
- Se usados incorretamente, podem atrapalhar ao invés de ajudar.


# UML Básico

Um diagrama representa as características de um objeto, divididas em atributos e operações.

Exemplos de diagrama:
![[Pasted image 20231221142100.png]]

Sinal de Menos é Private
Sinal de Mais é Public
Sinal de hashtag é Protected

![[Pasted image 20231221143546.png]]

Representação de Herança, onde Circle herda as características de Shape

![[Pasted image 20231221143802.png]]

Representação de Composição e Agregação

![[Pasted image 20231221143953.png]]

Representação de Dependência

![[Pasted image 20231221144101.png]]

Representação de Realization

![[Pasted image 20231221144601.png]]

Representação de uma Abstração
Classes abstratas não podem ser instanciadas diretamente

# Padrões de criação

Padrões que trabalham com a criação de objetos.
## Singleton

Intenção oficial - Garantir que uma classe tenha somente uma instância no programa e fornecer um ponto de acesso global para a mesma.

### Somente uma instância ?

- Geralmente usado para acesso a recursos compartilhados, como acesso à base de dados, interfaces gráficas, sistemas de arquivos, servidores de impressão, logger e mais.
- Também usado para substituir variáveis globais, como em casos de uso de objetos de configuração do sistema como um todo.

### Ponto de acesso global ?

- Você pode permitir acesso global ao Singleton em toda sua aplicação, assim como fazíamos (ou fazemos) com variáveis globais.
- Uma vantagem do Singleton é que podemos proteger a instância com encapsulamento, evitando que outro código sobrescreva seu valor.

### Aplicabilidade

- Use o Singleton quando uma classe precisa ter somente uma instância disponível e todo o seu programa.
- Use o Singleton quando perceber que está usando variáveis globais para manter partes importantes do programa, como variáveis de configuração que são usadas por toda a aplicação.

### Consequências

#### Bom

- Acesso controlado à instância única
- É fácil permitir um número maior de instâncias caso mude de ideia
- Usa Lazy instantiation, o Singleton só é criado no momento do uso
- Substitui variáveis globais

#### Ruim

- É mais difícil de testar
- Viola o princípio de responsabilidade única
- Requer tratamento especial em caso de concorrência
- Erich Gamma (autor) descreveu que esse seria o único padrão que ele removeria se fosse refatorar o livro - bit.ly/nosigleton

## Builder

Intenção oficial - Separar a construção de um objeto complexo da sua representação de modo que o mesmo processo de construção possa criar diferentes representações.

### Visão geral

- O padrão sugere a separação do código que cria e o código que usa o objeto
- Trata da criação de objetos complexos (complexos de verdade)
	- Construtores muito complexos
	- Composição de vários objetos (composite)
	- Algoritmo de criação do objeto complexo
- Permite a criação de um objeto em etapas
- Permite method chaining
- O objeto final pode variar de acordo com a necessidade
- É um padrão complexo

![[Pasted image 20240407155509.png]]

Builder - Define a interface de todos os objetos "Builder". As etapas de construção em comum são definidas aqui. (Pode ser uma classe abstrata ou interface)

Concrete Builder - Builders concretos implementam a interface de acordo com a sua necessidade. Elas podem produzir produtos de tipos deferentes.

Product - Os produtos finais são os objetos que o cliente deseja consumir. Eles não tem uma interface em comum porque podem ser de tipos diferentes.

Director - A classe "Director" é opcional. Ela pode definir a ordem em que as etapas de construção dos objetos são executadas.

Exemplo simples de builder e method chaining

![[Pasted image 20240407161203.png]]

### Consequências

#### Bom

- Separa criação de utilização
- O cliente não precisa criar objetos diretamente
- O mesmo código pode construir objetos diferentes
- Ajuda na aplicação dos princípios Single Responsability Principle e Open Closed Principle

#### Ruim

- O código final pode se tornar muito complexo