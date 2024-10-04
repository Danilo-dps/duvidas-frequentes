### Dúvidas

**O que é um web service?**

Um **web service** é uma tecnologia que permite a comunicação entre diferentes aplicações através da **internet**. Ele funciona como uma **ponte** que conecta sistemas distintos, independentemente da **linguagem de programação** ou **plataforma** que utilizam.

Existem dois principais tipos de web services:
1. **SOAP (Simple Object Access Protocol)**: Utiliza **XML** para enviar mensagens e geralmente opera sobre o protocolo **HTTP**. É conhecido por ser **robusto** e **seguro**, mas pode ser mais complexo de implementar.
2. **REST (Representational State Transfer)**: Utiliza o protocolo **HTTP** e permite a representação de dados em vários formatos, como **JSON** e **XML**. É mais **simples** e **flexível**, sendo amplamente utilizado atualmente.

Os web services são muito úteis para **integrar sistemas diferentes**, permitindo que compartilhem **dados** e **funcionalidades** de maneira eficiente. Por exemplo, um serviço de correios pode oferecer um web service que permite a consulta de endereços a partir de um **CEP**, facilitando a integração com outras aplicações.

**O que é uma API?**

Uma **API (Application Programming Interface)** é um conjunto de definições e protocolos que permite a comunicação entre diferentes sistemas de software. 
    Em português, **API significa Interface de Programação de Aplicações.**
    Aqui estão alguns pontos-chave sobre **APIs**:
    **Facilitam a Integração**: **APIs** permitem que diferentes sistemas e aplicações se comuniquem e compartilhem dados de forma padronizada, sem a necessidade de saber como cada sistema é implementado internamente.
    **Economia de Tempo e Recursos**: Com **APIs**, desenvolvedores podem reutilizar funcionalidades existentes em vez de criar tudo do zero. 
    Por exemplo, um aplicativo de mapas pode usar a **API do Google Maps** para integrar funcionalidades de mapeamento.
    **Segurança**: **APIs** podem controlar o acesso a dados e funcionalidades, garantindo que apenas usuários autorizados possam realizar determinadas ações.
    Um exemplo prático é quando você usa um aplicativo de clima no seu celular. 
    O aplicativo pode usar uma **API** para obter dados meteorológicos de um serviço externo e exibir essas informações para você.

**O que são microsserviços?**

**Microsserviços** são uma abordagem arquitetônica e organizacional do desenvolvimento de software na qual o software consiste em pequenos serviços independentes que se comunicam usando **APIs** bem definidas. 
Esses serviços pertencem a pequenas equipes autossuficientes.
As arquiteturas de **microsserviços** facilitam a **escalabilidade** e **agilizam** o desenvolvimento de aplicativos, habilitando a inovação e acelerando o tempo de introdução de novos recursos no mercado.
- [Saiba mais na AWS](https://aws.amazon.com/pt/microservices/)

**O que é conteinerização?**

A **conteinerização** é um processo de implantação de software que agrupa o **código** de uma aplicação com todos os **arquivos** e **bibliotecas** de que ela precisa para ser executada em qualquer **infraestrutura**. 

Tradicionalmente, para executar qualquer aplicação em seu computador, era necessário instalar a versão que correspondia ao **sistema operacional** da sua máquina. Por exemplo, você precisava instalar a versão **Windows** de um pacote de software em uma máquina Windows. 

No entanto, com a conteinerização, você pode criar um único pacote de software, ou **contêiner**, que é executado em todos os tipos de **dispositivos** e sistemas operacionais. 
- [Saiba mais na IBM](https://www.ibm.com/br-pt/topics/containerization)
- [Saiba mais na AWS](https://www.ibm.com/br-pt/topics/containerization)

**O que é Docker?**

**Docker** é uma plataforma de software **open source** que facilita a **criação**, **implantação** e **execução** de aplicações em **contêineres**. 

A tecnologia de **conteinerização** do Docker permite empacotar uma aplicação com todas as suas **dependências** em um único **contêiner**, garantindo que ela funcione de maneira **consistente** em qualquer **ambiente**.
- [Saiba mais na RedHat](https://www.redhat.com/pt-br/topics/containers/what-is-docker)

**O que significa uma API REST?**

Uma **API REST** (Representational State Transfer) é um tipo de interface de programação de aplicativos que segue princípios específicos para facilitar a comunicação entre sistemas através da **web**. Aqui estão alguns pontos principais sobre APIs REST:

- **Comunicação via HTTP**: As APIs REST utilizam os métodos **HTTP** (**GET**, **POST**, **PUT**, **DELETE**) para realizar operações de criação, leitura, atualização e exclusão de dados, conhecidas como operações **CRUD**.
- **Stateless**: Cada solicitação de um cliente para o servidor deve conter todas as informações necessárias para entender e processar o pedido. Isso significa que o servidor não armazena o estado da sessão do cliente entre as solicitações.
- **Formato de Dados**: Normalmente, as APIs REST utilizam **JSON** (JavaScript Object Notation) para trocar dados, devido à sua simplicidade e facilidade de uso.
- **Escalabilidade e Flexibilidade**: Devido à sua arquitetura, as APIs REST são altamente escaláveis e flexíveis, permitindo que diferentes componentes de software se comuniquem de maneira eficiente.

Essas características tornam as APIs REST uma escolha popular para a **integração de sistemas** e desenvolvimento de **aplicações web**.
- [Saiba mais na IBM](https://www.ibm.com/br-pt/topics/rest-apis) 
- [Saiba mais na RedHat](https://www.redhat.com/pt-br/topics/api/what-is-a-rest-api)

**Qual a diferença entre um web service, uma API e o microsserviço?**

## Web Service

Um **web service** é um tipo de **API** que opera através da **web**, permitindo a comunicação entre diferentes sistemas pela internet. Ele utiliza protocolos padrão como **SOAP** (Simple Object Access Protocol) ou **REST** (Representational State Transfer) para enviar e receber dados. 
Web services são projetados para serem **interoperáveis** entre diferentes plataformas e linguagens de programação.

## API (Application Programming Interface)

Uma **API** é um conjunto de definições e protocolos que permite que diferentes softwares se comuniquem entre si. As APIs podem ser usadas para acessar funcionalidades ou dados de um serviço, aplicativo ou sistema operacional. 
Elas não precisam necessariamente operar pela web; podem ser **locais** ou **remotas**. 
As **APIs RESTful** são um tipo comum de API web, mas existem muitas outras formas, como APIs de bibliotecas ou de sistemas operacionais.

## Microsserviço

Um **microsserviço** é uma abordagem arquitetural onde uma aplicação é dividida em pequenos serviços independentes, cada um executando uma função específica. 
Esses serviços são desenvolvidos, implantados e escalados de forma independente, o que facilita a manutenção e a escalabilidade do sistema como um todo. 
Microsserviços geralmente se comunicam entre si através de **APIs**, permitindo que cada serviço seja atualizado ou substituído sem afetar os outros.

## Resumo das Diferenças

- **Web Service**: Um tipo de API que opera pela web usando protocolos como SOAP ou REST.
- **API**: Um conjunto de definições e protocolos para comunicação entre softwares, que pode ou não operar pela web.
- **Microsserviço**: Uma abordagem arquitetural que divide uma aplicação em pequenos serviços independentes, que se comunicam via APIs.
- [Saiba mais na AWS](https://aws.amazon.com/pt/compare/the-difference-between-microservices-and-apis/)

**Qual a diferença entre uma API REST e uma API RESTful?**

# Diferença entre API REST e API RESTful

Há uma diferença sutil entre os termos **API REST** e **API RESTful**, embora muitas vezes sejam usados de forma intercambiável.

## API REST

Uma **API REST** é uma interface de programação de aplicativos que segue os princípios da arquitetura **REST** (Representational State Transfer). Ela utiliza métodos HTTP padrão (como **GET**, **POST**, **PUT**, **DELETE**) para realizar operações sobre os recursos, que são identificados por **URLs**. 
A comunicação geralmente é feita usando formatos como **JSON** ou **XML**.

## API RESTful

O termo **API RESTful** refere-se a uma API que não apenas segue os princípios da arquitetura **REST**, mas também adere estritamente às suas restrições e melhores práticas. 
Em outras palavras, uma API RESTful é uma implementação de uma API REST que é fiel aos princípios REST, como a separação entre cliente e servidor, a ausência de estado (**stateless**), a capacidade de **cache**, a interface uniforme, entre outros.

## Resumo das Diferenças

- **API REST**: Qualquer API que segue os princípios da arquitetura REST.
- **API RESTful**: Uma API que implementa os princípios REST de forma rigorosa e completa.

Em resumo, todas as APIs RESTful são APIs REST, mas nem todas as APIs REST são necessariamente RESTful, pois podem não seguir todas as restrições e melhores práticas da arquitetura REST.
- [Saiba mais na AWS](https://aws.amazon.com/pt/what-is/restful-api/)
