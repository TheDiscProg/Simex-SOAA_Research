# Mangaging Complexity and Security in Software Engineering

Many modern applications can suffer from complexity and security.

Software complexity can negatively impact maintenance, such as bug fixing and enhancement. It has been compared to a werewolf that results in "missed schedules, blown budgets and flawed products." This complexity arises mainly due to the abstraction of business models and is sometimes further complicated by the additional abstraction in Scala applications.

Data breaches have highlighted that Internet-facing application servers that connect to data sources, such as databases, are inherently unsafe.

This research paper looks at ways in which these two issues can be managed by using **Simple Exchange Message (Simex) API** and **Simex Oriented Asynchronous Architecture (SOAA)**.

As part of this research project, the following is a list of open-source Scala libraries that have been developed to support Simex and SOAA:

- **simex-messaging** Simex message with JSON encoders/decoders
- **slogic** - Provides **Xor** logic for use within *simex-messaging*
- **simex-util-library** - a utility library for use with web-based applications
- **simex-rabbitmq** - a RabbitMQ publisher and consumer for Simex messages
- **simex-kafka** - a Kafka publisher and consumber for Simex messages
- **simex-web-service** - a web service that handles Simex messages using HTTP POST methods
- **simex-cluster-caching** - a clustered caching service that can be used across instances for sharing data

These libraries are also available in Maven Central under [*io.github.thediscprog*](https://mvnrepository.com/artifact/io.github.thediscprog).

In addition, the research paper also details a network protocol, Simex Exchange Protocol or SEP for short, that can be used to enhance communication and security (currently in development).

**Please note that this is still in early draft.**
