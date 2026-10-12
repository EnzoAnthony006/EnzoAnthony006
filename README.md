<h1 align="center">Enzo Anthony</h1>

<p align="center">
  <b>Desenvolvedor Backend Java Jr.</b><br/>
  Spring Boot · Kafka · Redis · Docker · Testcontainers
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/enzo-anthony/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:enzoanthonydev06@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://enzoanthony006.github.io/Portf-lio-EnzoAnthony/"><img src="https://img.shields.io/badge/Portfólio-FF6F3C?style=for-the-badge&logo=googlechrome&logoColor=white"/></a>
</p>

## 👋 Sobre

Construo APIs em Java e Spring Boot que vão além do CRUD: **mensageria**, **cache**, **segurança com OAuth2/Keycloak**, **testes com Testcontainers**, **CI** e **observabilidade**. Estudo backend por conta própria desde novembro de 2025, curso Sistemas de Informação na Impacta e sou Jovem Aprendiz em TI na ACT Digital.

**🔎 Buscando minha primeira oportunidade como Estagiário ou Desenvolvedor Backend Java Jr em São Paulo (presencial, remoto ou híbrido).**

## 🏦 Projeto em destaque: [Cofrinhos API](https://github.com/EnzoAnthony006/cofrinhos-api)

App de economia gamificada: você cria cofrinhos (metas), registra aportes e ganha XP, nível, sequência semanal e conquistas, com um **ranking que atualiza ao vivo**.

```mermaid
flowchart LR
    A["Aporte (API REST)"] --> B[("PostgreSQL")]
    A --> C{{"Kafka: aporte-registrado"}}
    C --> D["Consumidor"]
    D --> E["XP, nível e conquistas"]
    D --> F[("Redis: ranking")]
    F --> G["SSE ao vivo no navegador"]
```

- **Arquitetura hexagonal com DDD**, com o domínio isolado de framework
- **Kafka** para processar XP e conquistas de forma assíncrona, sem travar a API
- **Redis** (cache e ranking em sorted set) e **WebFlux/SSE** para tempo real
- **OAuth2 + Keycloak**, com cada usuário acessando apenas os próprios dados
- **Mais de 80 testes** (JUnit 5, Mockito, Testcontainers), CI no GitHub Actions e traces no Jaeger

## 📂 Outros projetos

| Projeto | O que resolve | Tecnologias |
| --- | --- | --- |
| [Payment Gateway](https://github.com/EnzoAnthony006/payment-gateway-service) | Falhas de um provedor instável e cobrança duplicada | Resilience4j, RabbitMQ, PostgreSQL, Testcontainers |
| [Notification Service](https://github.com/EnzoAnthony006/notification-service) | Acoplamento entre serviços com comunicação assíncrona | Kafka, Clean Architecture, GitHub Actions |
| [URL Shortener](https://github.com/EnzoAnthony006/url-shortener) | Consulta repetida ao banco a cada redirecionamento | JWT, Redis, Docker |
| [Gestão Acadêmica](https://github.com/EnzoAnthony006/gestao-academica-api) | Controle de acesso por perfil com front-end integrado | JWT, 3 roles, MySQL, ViaCEP |

## 🛠️ Stack

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=flat&logo=keycloak&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white)

| Área | Tecnologias |
| --- | --- |
| Backend | Java 17/21, Spring Boot 3/4, Spring Security, JPA, WebFlux, Maven |
| Dados e mensageria | PostgreSQL, MySQL, Redis, Flyway, Kafka, RabbitMQ |
| Segurança | OAuth2, Keycloak, JWT, Resilience4j |
| Testes e DevOps | JUnit 5, Mockito, Testcontainers, Docker Compose, GitHub Actions, OpenTelemetry (Jaeger) |
| Cloud | AWS (EC2, S3, RDS, Lambda, VPC, IAM), Google Cloud, fundamentos de Kubernetes |

## 📚 Estudando agora

gRPC e protocolos entre microsserviços · Outbox pattern · Kubernetes na prática · Logs com Loki

## 🏆 Certificações

AWS Academy Cloud Architecting (+50h de labs) · AWS Cloud Practitioner Essentials · AWS Technical Essentials · AWS Cloud Quest: IA Generativa · Google Cloud Digital Leader · Bootcamp CI&T Backend Java e AWS

---

<p align="center">📬 <a href="mailto:enzoanthonydev06@gmail.com">enzoanthonydev06@gmail.com</a> · <a href="https://www.linkedin.com/in/enzo-anthony/">linkedin.com/in/enzo-anthony</a></p>
