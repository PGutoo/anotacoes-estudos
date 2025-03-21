## @SpringBootApplication
Combinação de outras anotações, uma estrutura que determina a classe que inicia a aplicação

## @EnableAutoConfiguration
Configura automaticamente configurações padrões do spring, como o tomcat

## @ConfigurationProperties
Determina atraves de prefixos quais valores buscar pelo arquivo de propriedades, se por exemplo tiver prefixo "app", vai pegar os valores correspondente desse app dentro do arquivo properties e atribuir por exemplo à atributos de uma classe, de acordo com o nome desses atributos
app.name=pedro
atributo -> name = pedro
