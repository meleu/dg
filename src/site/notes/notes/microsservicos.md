---
{"dg-publish":true,"permalink":"/notes/microsservicos/"}
---

# Estudando Microsserviços

## Referências

- [[notes/videos/Microservices - Codigo Fonte TV\|Microservices - Codigo Fonte TV]]
- [[notes/videos/O que sao Microsservicos - Alura\|O que sao Microsservicos - Alura]]
- [[notes/videos/Martin Fowler - Microservices\|Martin Fowler - Microservices]]
- [[notes/videos/The Problem with Microservices - Dave Farley\|The Problem with Microservices - Dave Farley]]
- [[notes/videos/Microsservicos muito alem da teoria - Andre Nobre\|Microsservicos muito alem da teoria - Andre Nobre]]
- [[notes/videos/When To Use Microservices - Sam Newman\|When To Use Microservices - Sam Newman]]
- [[notes/videos/Pragmatic Microservices - Randy Shoup\|Pragmatic Microservices - Randy Shoup]]
- [[notes/videos/Interview with Sam Newman about Microservices\|Interview with Sam Newman about Microservices]]
- [[notes/videos/Mastering Chaos - A Netflix Guide to Microservices\|Mastering Chaos - A Netflix Guide to Microservices]]
- [[notes/videos/Evolutionary Architecture and Microservices - Rebecca Parsons\|Evolutionary Architecture and Microservices - Rebecca Parsons]]


## Design Microservice Architectures the Right Way

- <https://www.youtube.com/watch?v=j6ow-UemzBc>

- parei em 19 minutos




## Microservices + Events + Docker = A Perfect Trio

- <https://youtu.be/sSm2dRarhPo>




## Minhas Palavras

### Definição de Arquitetura de Microsserviços

É uma forma de desenvolver sistemas de software onde cada pedaço pode ser pensado, desenvolvido e disponbilizado de forma independente.

> Microsserviços é um tipo de SOA

O paradigma de microsserviços é, digamos, inspirado no SOA (Service Oriented Architecture - Arquitetura Orientada a Serviços).

Eu arriscaria dizer que microsserviços é uma maneira mais específica e detalhada de praticar o Arquitetura Orientada a Serviços.

A gente vai ver também nessa apresentação como que as ferramentas de DevOps são o que dá sustentação para uma arquitetura de microsserviços. É o que torna humanamente viável a prática de microsserviços.


### Características de Microsserviços

- Utilizadas para tornar aplicações grandes e complexas mais digeríveis
- Utilizadas para tornar coordenação de times menos custosa.
- Deploy independente.
    - o que só é viável devido às técnicas de CI/CD, que automatizam esse processo
- Interfaces bem definidas (detalhes de implementação ficam encapsulados).

### desafios

Cada pedacinho do sistema separado (ou seja, o microsserviço) torna mais fácil a compreensão de cada um desses pedacinhos, facilitando a manutenção e implementação de melhorias desse pedacinho. Mas o sistema como um todo fica bem mais complexo.

É necessário termos uma boa gestão e orquestração desses microsserviços para garantir um bom funcionamento do sistema como um todo.

### Quando/Por que utilizar Microsserviços?

- Aplicações grandes
- Muitos programadores trabalhando na mesma base de código.

**Observação**: a carga de trabalho, e portanto o custo operacional de implementar microsserviços aumenta consideravelmente


## Top 25 Microservice Interview Questions Answered - Java Brains

- <https://youtu.be/o36vWQCRrp0>