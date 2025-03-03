# Reducing Complexity whilst Maintaining Security in Software Engineering

**Please note that this is still in early draft.**

This document is an early draft and will undergo significant revisions as the API is developed and refined, including the title of the document.

## What's it about?
Software engineers encounter two fundamental challenges:
1. Complexity, both in the design of the application and the network communication between services and clients;
2. Protecting services from unauthorised access and information leakage.

## Complexity
In his 1986 paper titled “No Silver Bullet: Essence and Accidents of Software Engineering,” Frederick Brooks employed the metaphor of a werewolf to illustrate the detrimental effects of complexity on software maintenance and enhancement. This complexity manifests in missed deadlines, overspending, and subpar product quality. The primary source of complexity lies in the abstraction of business models, which can be further exacerbated by additional abstractions in functional programming.

This issue is further compounded by the complexity of network communications. For instance, numerous mobile applications access backend services via REST APIs through a gateway that corresponds to the URL of a backend service. Any modifications to the API requires updates to the client, backend services, and the gateway. Coordinating these changes can, at best, result in the dreaded 404 error or, at worst, expose the backend services.

## Software Security
Data breaches have underscored the inherent vulnerability of Internet-facing application servers that connect to data sources, such as databases, that store confidential data.

## How Does this paper help?
This paper looks at ways in which these two issues can be managed by using **Simple Message Exchange (Simex) API** and **Simex Oriented Asynchronous Architecture (SOAA)**. Although not claiming to be a "silver bullet," it can be a "silver-coated bullet."

As part of this project, the following is a list of open-source Scala libraries that have been developed to support Simex and SOAA:

- **simex-messaging** Simex message with JSON encoders/decoders
- **slogic** - Provides **Xor** logic for use within *simex-messaging*
- **simex-util-library** - a utility library for use with web-based applications
- **simex-rabbitmq** - a RabbitMQ publisher and consumer for Simex messages
- **simex-kafka** - a Kafka publisher and consumber for Simex messages
- **simex-web-service** - a web service that handles Simex messages using HTTP POST methods
- **simex-cluster-caching** - a clustered caching service that can be used across instances for sharing data

These libraries are also available in Maven Central under [*io.github.thediscprog*](https://mvnrepository.com/artifact/io.github.thediscprog).

Additionally, the research paper outlines a network protocol, the Simex Exchange Protocol (SEP), which can be employed to augment communication and enhance security (currently in the early development phase).

