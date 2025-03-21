# Monitoramento Universal de Serviço

O Monitoramento Universal de Serviço (USM) oferece uma visão das métricas de saúde de serviços em toda a sua pilha tecnológica, sem a necessidade de instrumentar seu código. Em vez disso, ele depende da presença de um Agente Datadog configurado e da Tagueamento de Serviço Unificado para coletar dados sobre seus serviços existentes, que podem então ser visualizados através do Catálogo de Serviços.

Para habilitar o USM, são necessários os seguintes requisitos:

- Se estiver usando Linux, o serviço deve estar rodando em um contêiner.
- Se estiver usando Windows e IIS, o serviço deve estar rodando em uma máquina virtual.
- O Agente Datadog precisa estar instalado junto ao seu serviço.
- A tag **env** para o Tagueamento de Serviço Unificado deve ser aplicada à sua implantação.

# Tagueamento Unificado de Serviços

O Monitoramento Universal de Serviços é capaz de identificar serviços por meio de tags de contêiner comumente usadas (como **app**, **short_image** e **container_name**), gerando automaticamente entradas correspondentes no Catálogo de Serviços.

Uma vez que esses serviços são descobertos, o Datadog permite acessar métricas de requisição, erro e duração tanto para o tráfego de entrada quanto de saída. Essas métricas de saúde de serviço são úteis para configurar alertas, rastrear implantações e estabelecer objetivos de nível de serviço (SLOs), fornecendo uma visão abrangente de todos os serviços que estão rodando na sua infraestrutura.