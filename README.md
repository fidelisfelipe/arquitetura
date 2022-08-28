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






