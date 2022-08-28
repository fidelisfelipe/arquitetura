# Design e Arquitetura de Software

Este é um guia de assuntos relacionados a arquitetura de softwares.

# Paradigmas de Programação

**Software**: Matéria vital dos programas de computadores.
 É sequência, seleção, iteração e indireção. Nada mais e nada menos.
 
**Programação estruturada**
  - Disciplina imposta sobre a transferência direta de controle
  - Sequencial e Convencional

**Orientação a Objetos**
  - Disciplina imposta sobre a transferência indireta de controle
  - Plugins
  - Polimorfismo - Ponteiro em Funções - desde o fim da década de 1940 por Von Neumann
  - Inversão de Depêndencia
  - Desenvolvimento Independente
  - Implantação Independente

**Programação Funcional**
  - Disciplina imposta sobre atribuição de variáveis
  - Imutáveis - Create and Read

# Arquitetura Orientada a Serviço (SOA)

**Web Services**

>Em grandes empresas ou organizações, o código interno pode ser transformado em serviços
que podem ser usados por diferentes partes das empresas ou combinando mais dois serviços.
Esses serviços podem ser criados do zero ou adicionando interfaces ao software existente.

Uma vez implementados, os serviços podem ser usados para impulsionar os objetivos da empresa ou da organização.
**Ele deve ser:** Modular, Combinável, Independente de Plataforma, Idioma, Auto-descritivo, Catalogado.

> **Vamos olhar para trás?** 
> - *Em 1969, o antecessor da Internet, uma pequena rede de computadores chamada ARPANET, foi usado por pesquisadores nos Estados Unidos para enviar uma pequena quantidade de dados
entre pares de computadores. Esta foi a primeira vez que os dados foram enviados através de uma rede de computadores.* 
> - *Tim Berners-Lee começou a investigar como os documentos poderiam ser ligados entre si
através de redes. Em 1990, Lee propôs um sistema de gerenciamento web inspirado no hipertexto e
construído sobre a Internet, chamado World Wide Web. A World Wide Web, também conhecida como web, levou a padrões e tecnologias para comunicação baseada em computador através da Internet.*

**HTML**- *O texto nas páginas da Web é estruturado por meio de uma linguagem de marcação, HyperText Markup Language.*
**XML**- *É uma linguagem de marcação destinada a armazenar e transportar dados, Extensible Markup Language.*
**JSON**- *Formato que pode ser usado para armazenar e transportar dados, JavaScript Object Notation.*
**HTTP**-*HTTP é um protocolo que determina como a informação, incluindo o hipertexto, é transferida através da Internet. Existem várias versões de protocolo.*
**URI**-*Identificadores de recursos universais, são endereços usados para identificar recursos.*
**URL**-*Localizadores de Recursos Universais, são um subconjunto de URIs que são usados para localizar recursos. Ambos são usados para identificar o recurso, mas URLs também dizem ao protocolo como localizar e acessar o recurso*

**Remote Procedure Call (RPC)**
> *Chamadas de Procedimento Remoto*- O RPC foi projetado especificamente como um componente de middleware para
sistemas em rede e foi estendido para melhorar sua flexibilidade e usabilidade. Como o nome indica, uma chamada de procedimento remoto permite que os clientes invoquem procedimentos que são implementados em um servidor.
Aqui, o cliente e o servidor estão em máquinas completamente separadas ou são uma instância virtual diferente na mesma máquina. 

**Object Brokers**
> *CORBA*-A arquitetura de agente de objeto mais comum é chamada de Arquitetura Common Object Request Broker. Apesar de ter a palavra arquitetura em seu nome, CORBA está mais intimamente relacionado com um conjunto de padrões. Concebido pelo Grupo de Gerenciamento de Objetos, ou OMG, o CORBA tem como objetivo fornecer um esboço do que deve ser incluído em corretores de objetos. O padrão não é um guia de instruções para implementação.
Como existem inúmeras linguagens orientadas a objetos, o principal objetivo da CORBA é criar uma especificação que permita que os corretores de objetos sejam independentes das linguagens de programação usadas para implementar clientes e servidores. CORBA especifica que os corretores de objetos devem ser capazes de funcionar independentemente do sistema operacional. 
A intenção é que, se um sistema requer middleware para manipular a computação distribuída, os desenvolvedores não precisam ser restritos aos requisitos de idioma e sistema operacional do middleware.

**Web Services de primeira geração**
> *O que é*-Um serviço é alguma funcionalidade que é exposta para uso por outros processos. Em outras palavras, um serviço tem uma interface que pode ser usada por algum solicitante de serviço. Um serviço Web, então, é uma funcionalidade que é exposta e acessível usando tecnologias da Web.

> Quais são alguns dos motivos pelos quais o Enterprise Application Integration (EAI) não é comumente usado em cenários business-to-business (B2B)?

> - Não é óbvio onde colocar o middleware

> - As empresas querem manter o controle sobre seus dados

> - A segurança pode ser um problema

**Como são chamados?** 
> Para que um solicitante de serviço use um serviço específico, ele deve chamá-lo. Invocar é como uma chamada de método em uma linguagem orientada a objeto, exceto que ele deve ser feito através de uma solicitação em XML. A invocação incluirá qual operação é solicitada, uma vez que um serviço pode oferecer vários, juntamente com os parâmetros em Dados. Na invocação de serviços Web é feita com SOAP, uma especificação de protocolo que é baseada em XML e permite que os serviços enviem informações uns aos outros. SOAP ao mesmo tempo representava Simple Object Access Protocol. Embora este significado tenha sido descartado. Solicitantes de serviço e provedores de serviços usam essas mensagens SOAP para enviar informações uns aos outros. Uma vez que as mensagens são baseadas em XML e enviadas através de infraestrutura web universalmente aceita, sistemas codificados em diferentes idiomas e em diferentes plataformas podem facilmente se comunicar.

**Como são descritos?**
> Para que os serviços interajam, eles devem saber como interagir. Linguagens de descrição do serviço Web ou WSDL é o protocolo padrão para descrever a interface de um serviço. Como SOAP, as descrições WSDL são escritas em XML. Uma descrição WSDL descreverá a interface de um serviço de forma legível por máquina para que um solicitante de serviço possa se vincular a essa interface. Vinculação é o ato de gerar o código necessário para interagir com um serviço para que um solicitante de serviço possa começar a chamá-lo. Se uma interface de serviço é descrita de forma inequívoca com WSDL, a vinculação pode ser feita gerando o código necessário automaticamente.

**Como são publicados e descobertos?**
> A internet é um lugar grande, solicitantes de serviços e prestadores de serviços precisam de maneiras de entrar em contato. Os provedores de serviços podem publicar descrições de seus serviços usando UDDI, descrição universal, descoberta e integração. UDDI é usado para construir registros públicos ou privados de serviços web. Solicitantes de serviço que procuram um serviço podem pesquisar pelas descrições WSDL ou outros aspectos do serviço. Isso é chamado de descoberta, juntos SOAP, WSDL e UDDI são os três padrões fundamentais de serviços web. Eles permitem que os serviços Web sejam invocados por solicitantes de serviço, para se descrever e para ser publicado registros onde eles podem ser descobertos. Todos eles dependem da infraestrutura da Web.

**Como são combinados:**
> Composição é a ação de coordenar vários serviços e fornecer uma interface. A reutilização pode ser alcançada por agregação.
> No contexto de webservices seria determinar a ordem e lidar com exceções que podem surgir podendo ser chamado de coordenação.
> *BPEL* - Businnes Process Execution Language - Linguagem padrão de composição de alto nível para serviços web.

*Quais são os três padrões fundamentais dos Web Services de primeira geração?*

> - WSL é a especificação para descrever interfaces de serviço da web.
> - SOAP é o padrão usado para invocar serviços da web - Robusto, Modular e Extensível.
> - A UDDI reúne provedores de serviços e solicitantes de serviços, oferecendo publicação e descoberta.

###SOAP
> - Simple Object Access Protocol -  é um protocolo padrão projetado originalmente para possibilitar a comunicação entre aplicações desenvolvidas em diferentes linguagens e plataformas.

**Estilo comum para invocações SOAP**

> - *RPC* - O estilo de chamada de procedimento remoto se parece com uma chamada de método, onde você invoca um processo e passa parâmetros. No entanto, eles não são como uma simples chamada de método em OO, pois precisam de muitas informações extras, como o protocolo de transporte.

> - *Document* - Nesse estilo, o tipo de formulário enviado informa ao serviço o que fazer e os campos no formulário são como os parâmetros são passados.

*Comunicação Default SOAP*
```mermaid
graph LR
A[client code] --> B[client stub] --> C[SOAP engine] --> D[HTTP engine] --> 
E[HTTP server] --> F[SOAP router] --> G[server stub] --> H[service code]
```
**Existem quatro padrões básicos de mensagens possíveis com SOAP**

*Request-Response*
>O padrão de resposta da solicitação é quando o solicitante do serviço envia pela primeira vez uma mensagem, em seguida, recebe uma resposta do provedor de serviços.
> Este processo é síncrono. Ele pode ser implementado através de HTTP.
> Inerentemente síncrono.
```mermaid
graph LR
A[Service Requester] --request--> B[Service Provider]
B --response--> A
```
*Solicitation-Response*
>Também é síncrona, o provedor de serviços, faz uma solicitação para o solicitante do serviço. Isso geralmente é uma confirmação.
```mermaid
graph LR
A[Service Provider] --solicitation--> B[Service Requester]
B --response--> A
```
*One-Way*
>No padrão de comunicação unidirecional, o solicitante de serviço envia uma solicitação para o provedor de serviços, as nenhuma resposta é esperada. Isso pode ser uma notificação simples de que o solicitante do serviço está ativo e em execução.
>Esse padrão é inerentemente assíncrono, uma vez que nenhuma resposta é esperada.
```mermaid
graph LR
A[Service Requester] --request--> B[Service Provider]
```
*Notification*
>No padrão de mensagem de notificação, o provedor de serviço envia uma notificação para o solicitante sem esperar uma resposta. Este modelo é adequado para sistemas baseados em eventos, onde há editores e assinantes, como um blog ou um serviço de notificação meteorológica.
>Esse padrão de mensagens também é assíncrono.
```mermaid
graph LR
A[Service Provider] -- notification--> B[Service Requester]
```

### UDDI
> - Universal Description, Discovery and Integration, Descrição, Descoberta e Integração Universais - Lançado em 2000, define um padrão de publicar e descobrir informações sobre serviços da Web.
> Hoje, gerenciado pela OASIS. Não é um componente obrigatório para implementação de serviços web. Tem o papel de Reunir provedores de serviços e solicitantes de serviços mas também tem o papel de publicar e manter esses serviços.
> As informações ~soa divididas em 3 categorias: 
> - Páginas brancas - Informações básicas sobre o negócio como nome, descrição e telefone.
> - Páginas amarelas - Informações hierarquicas sobre o serviço da empresa e subconjuntos.
> - Páginas verdes - Informações técnicas de como utilizar o serviço.
> O UDDI permite que os serviços sejam publicados e descobertos, mas um registro UDDI também é um provedor de serviços!
> Alguns dos serviços que oferece são adicionar negócios ou serviços ou alterar informações sobre serviços.