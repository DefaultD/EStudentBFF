📘 EStudentBFF

O EStudentBFF (Backend for Frontend) é o gateway de comunicação entre o frontend da plataforma EStudent e os microserviços internos que compõem o ecossistema escolar.
Ele centraliza as chamadas para os serviços de aluno, professor, matrícula, boletim, financeiro e demais módulos, aplicando regras específicas de apresentação e agregação de dados voltadas à experiência do usuário.

🚀 Principais responsabilidades

Intermediar a comunicação entre o frontend e os microserviços (Student, Class, Finance, etc).

Agregar e transformar dados vindos de múltiplas APIs.

Garantir segurança e controle de acesso via JWT/OAuth2.

Implementar caching e rate limiting para otimizar performance.

Padronizar respostas e reduzir a complexidade do cliente.

Realizar persistência leve de dados via Prisma ORM (ex: logs, cache persistente, tokens, etc).

🛠️ Stack principal

Node.js (NestJS / Express)

TypeScript

Prisma ORM (PostgreSQL / MySQL)

Axios / gRPC / GraphQL

Redis (cache em memória)

Jest (testes unitários e de integração)

🧱 Arquitetura

Segue princípios de Clean Architecture e Domain-Driven Design (DDD).

Estruturado em camadas (application, domain, infrastructure, presentation).

Cada contexto de negócio é representado como um módulo isolado (ex: students, teachers, classes).

O acesso a dados é abstraído via repositórios implementados com Prisma.

📦 Futuras implementações

Observabilidade (Prometheus + Grafana)

Circuit breaker e retry policy nas chamadas de serviço

Logging distribuído (ELK stack)

🧠 Parte do ecossistema EStudent, um sistema escolar modular construído com foco em escalabilidade e boas práticas de arquitetura de software.
