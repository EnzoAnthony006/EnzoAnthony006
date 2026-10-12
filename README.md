<h1 align="center">Olá, eu sou o Enzo Anthony</h1>

<p align="center">
  <b>Desenvolvedor Backend Java Jr. · Spring Boot · Kafka · Redis · Docker</b><br/>
  Estudante de Sistemas de Informação · Jovem Aprendiz em TI @ACT Digital
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/enzo-anthony/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:enzoanthonydev06@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://github.com/EnzoAnthony006" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <a href="https://enzoanthony006.github.io/Portf-lio-EnzoAnthony/" target="_blank">
    <img src="https://img.shields.io/badge/Portfólio-FF6F3C?style=for-the-badge&logo=googlechrome&logoColor=white"/>
  </a>
</p>

---

## 👋 Sobre mim

Construo APIs em Java e Spring Boot pensando no que vem depois do CRUD: **mensageria** (Kafka e RabbitMQ), **cache** (Redis), **segurança** (JWT, OAuth2 com Keycloak), **resiliência** (Circuit Breaker e Retry), **testes de integração** (Testcontainers), **CI** (GitHub Actions) e **observabilidade** (Prometheus, Grafana, OpenTelemetry e Jaeger).

Estudo backend de forma autodidata desde novembro de 2025 e transformo o que aprendo em projetos que rodam de verdade, com testes e pipeline. Sou Jovem Aprendiz em TI na **ACT Digital** (Barueri/SP) e tenho mais de **50 horas de prática em AWS** (AWS Academy Cloud Architecting) e o **Google Cloud Digital Leader**.

**🔎 Buscando minha primeira posição como Estagiário ou Desenvolvedor Backend Java Jr, em São Paulo (presencial, remoto ou híbrido).**

---

## 🚀 Projeto em destaque

### 🏦 [Cofrinhos API](https://github.com/EnzoAnthony006/cofrinhos-api)

![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=flat&logo=keycloak&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat&logo=opentelemetry&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

Aplicação de economia **gamificada**: você cria cofrinhos (metas de poupança), registra aportes e ganha **XP, nível, sequência semanal e conquistas**, com um **ranking que atualiza ao vivo**.

- **Arquitetura hexagonal com DDD**, com o domínio isolado de framework
- **Kafka:** cada aporte vira um evento e a gamificação roda de forma assíncrona (consistência eventual)
- **Redis:** cache de leitura e ranking em sorted set; o ranking pode ser reconstruído a partir do banco
- **Segurança:** OAuth2 Resource Server com Keycloak; PKCE no front-end; cada usuário só acessa os próprios cofrinhos
- **Tempo real:** WebFlux e SSE para o ranking, lido com `fetch` porque o `EventSource` não envia o header `Authorization`
- **Observabilidade:** Prometheus, Grafana e traces no Jaeger via OpenTelemetry
- **Qualidade:** mais de 80 testes (JUnit 5, Mockito, Testcontainers), migrations com Flyway e CI no GitHub Actions
- **Front-end** em HTML, CSS e JavaScript puros, servido pelo próprio Spring

```
Aporte → API → Kafka → consumidor → XP + conquistas + ranking (Redis) → SSE → navegador
```

---

## 📂 Outros projetos

### 💳 [Payment Gateway Service](https://github.com/EnzoAnthony006/payment-gateway-service)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat&logo=rabbitmq&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white)

Gateway de pagamentos simulado em Clean Architecture, com foco em **resiliência** a falhas de um provedor externo instável: Circuit Breaker e Retry (Resilience4j) evitam que uma falha pontual derrube a aplicação, e idempotência garante que reenviar a mesma requisição não gera cobrança duplicada. Testes de integração com Testcontainers (Postgres e RabbitMQ reais) rodam no CI a cada push, e as métricas de latência e erro ficam visíveis no Grafana.

### 📬 [Sistema de Notificações](https://github.com/EnzoAnthony006/notification-service)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat&logo=apachekafka&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)

Notificações assíncronas com Apache Kafka e Clean Architecture: se um consumidor cai, o producer continua publicando sem impacto. O pipeline com GitHub Actions roda os testes (JUnit 5) e publica a imagem no Docker Hub a cada push.

### 🔗 [URL Shortener API](https://github.com/EnzoAnthony006/url-shortener)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

Encurtador de URLs com JWT stateless e controle de acesso. O cache com Redis serve a URL mais acessada direto da memória, sem consultar o banco a cada redirecionamento. Docker, testes com JUnit 5 e Mockito, documentação com Swagger.

### 🎓 [Gestão Acadêmica API](https://github.com/EnzoAnthony006/gestao-academica-api)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat&logo=springsecurity&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat&logo=swagger&logoColor=black)

API REST com JWT e 3 roles (`ADMIN`, `ALUNO`, `PROFESSOR`), cada uma com permissões diferentes. Front-end integrado com login e rotas protegidas, CORS resolvido entre front e back, e enriquecimento de endereço via ViaCEP.

<details>
<summary><b>Mais projetos</b></summary>

- 🔐 [Secure REST API](https://github.com/EnzoAnthony006/spring-securityjwt): JWT e roles (`USER`/`MANAGER`) com Spring Security, JPA e MySQL.
- 🌐 [API REST Clientes e Endereços](https://github.com/EnzoAnthony006/API-REST-Clientes-e-Enderecos): CRUD com validações e preenchimento de endereço pelo ViaCEP.

</details>

---

## 🛠️ Tecnologias

### ☕ Backend
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat&logo=springsecurity&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=flat&logo=keycloak&logoColor=white)
![JPA](https://img.shields.io/badge/JPA/Hibernate-59666C?style=flat&logo=hibernate&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat&logo=swagger&logoColor=black)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat&logo=apachemaven&logoColor=white)

### 🗄️ Dados e mensageria
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat&logo=apachekafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat&logo=rabbitmq&logoColor=white)

### 🧪 Testes e qualidade
![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=flat&logo=junit5&logoColor=white)
![Mockito](https://img.shields.io/badge/Mockito-78A641?style=flat&logoColor=white)
![Testcontainers](https://img.shields.io/badge/Testcontainers-2496ED?style=flat&logo=docker&logoColor=white)

### 🐳 DevOps e observabilidade
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat&logo=opentelemetry&logoColor=white)

### ☁️ Cloud
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white)
![GCP](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=googlecloud&logoColor=white)

EC2 · S3 · RDS · Lambda · VPC · IAM · CloudFormation · CloudWatch · Auto Scaling · Load Balancer · Well-Architected Framework (labs do AWS Academy Cloud Architecting)

---

## 📚 Em estudo atualmente

gRPC e protocolos de comunicação entre microsserviços · Outbox pattern e consistência em eventos · Resilience4j entre serviços · Kubernetes na prática · Logs com Loki

**Próximo projeto:** Cofrinhos v2, com a gamificação em um serviço separado.

---

## 🏆 Certificações

| Badge | Certificação |
|---|---|
| ☁️ | [AWS Cloud Practitioner Essentials](https://www.credly.com/badges/6ae9c931-4575-4d30-b3fe-a5224a3a5c01/linked_in_profile) |
| ☁️ | AWS Technical Essentials |
| 🤖 | [AWS Cloud Quest: IA Generativa Practitioner](https://www.credly.com/badges/15cb87a5-f818-4848-a01c-815b6af74038) |
| 📐 | [AWS Academy Cloud Architecting — Módulos 2–16](https://www.credly.com/badges/4ec6ba6e-c4f5-48d6-8f7d-808216c6bbf9/public_url) |
| ☁️ | Google Cloud Digital Leader — trilha concluída |
| 🚀 | Bootcamp CI&T — Backend com Java e AWS |
| ☕ | Java — Criando uma Aplicação Completa (Impacta) |
| 🐙 | Contribuindo em Projetos Open Source no GitHub (DIO) |

---

<div align="center">
  <b>📬 Vamos conversar?</b><br/>
  <a href="mailto:enzoanthonydev06@gmail.com">enzoanthonydev06@gmail.com</a> ·
  <a href="https://www.linkedin.com/in/enzo-anthony/">linkedin.com/in/enzo-anthony</a>
</div>
