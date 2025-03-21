Grupo Beans:

## @AutoWired
 Indica ao Spring quando fazer injeção de uma dependencia. Por exemplo se faço uso dos métodos de uma classe Service em outra classe
 Evitando por exemplo fazer injeção através de um método construtor

## @Qualifier
 Quando mais de uma classe implementa uma interface é necessário indicar ao Spring qual implementação será usada naquela injeção
 Usando a seguinte sintaxe @Qualifier("nomeDaClasse"). O nome da classe entre aspas deve começar com letra minuscula.

## @Value
 Permite recuperar o valor de uma propriedade (Do arquivo application.properties ou application.yml) e define esse valor para um atributo
 Sintaxe: @Value("${caminho da propriedade indicada no arquivo"}).

Grupo Context:

## @Configuration
 Quando usada em uma classe o Spring leva em consideração as configurações indicadas por essa classe (Também indica que a classe é um bean, mesmo não sendo do Stereotype)

## @ComponentScan
 Indica ao Spring qual pacote na qual ele vai varrer e identificar quais os beans ele vai gerenciar
 Sintaxe: @ComponentScan(basePackages = "caminho do pacote"), por padrão ele determina o pacote raiz (É possivel excluir pacotes também)
 Essa anotação pode ser usada para customização de quais beans o Spring deve gerenciar, contudo, por natureza do Spring Boot ele já faz o ComponentScan do projeto como um todo

## @Bean
Permite a criação de beans a partir de outras classes, essas classes podem não possuir anotações. O @bean precisa estar dentro de uma classe com o @configuration, caso contrário, não será reconhecido aquele bean e dará erro.
Pode-se usar também para declarar beans de bibliotecas externas

## @Lazy
Quando um bean é criado e só é necessário utilizar em determinado momento, o lazy ajuda o spring a identificar quais beans se encaixam nesse caso

## @Primary
Declara prioridade para o bean, por exemplo, em classes de implementação para interfaces com mais de uma implementação

## @Scope
Permite ao Spring entender como ele vai lidar com o bean, se vai ser sigleton, prototype, 

## @PropertySource
Indica uma nova fonte de propriedade de arquivos .properties ou .yml, além do já criado por padrão pelo spring.
Se tivessemos multiplos arquivos de propriedade, basta usar o @propertysources, no plural

## @Profile
Permite identificar um recurso, como um método ou classe, sobre qual é o perfil dele, dev, hom, prod