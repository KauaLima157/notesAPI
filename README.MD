# Notes API

Backend de uma plataforma de notas e tarefas inspirada em ferramentas como Notion, com foco em organização por tags, histórico de alterações e arquitetura escalável.

Este projeto foi pensado como um **estudo aprofundado de backend**, priorizando boas práticas de arquitetura, versionamento e evolução incremental do sistema.

---

## Objetivo do Projeto

Construir uma API robusta para gerenciamento de notas e tarefas, explorando conceitos exigidos em ambientes profissionais, como:

* CRUD complexo
* Autenticação e autorização
* Separação clara de responsabilidades
* Evolução para arquitetura orientada a eventos
* Escalabilidade e manutenibilidade

---

## Stack Principal

* **Node.js**
* **TypeScript**
* **Express**
* **PostgreSQL** 
* **Redis** (cache, rate limit, sessões)

### Planejado para o futuro

* **RabbitMQ** (processamento assíncrono e eventos)
* **Docker**
* **CI/CD**

---

## 📁 Estrutura do Projeto

```
notesApi/
├── backend/
│   ├── docs/                 # Documentação técnica e decisões de arquitetura do backend
│   ├── scripts/              # Scripts utilitários (migrations, seeds, etc.)
│   ├── src/
│   │   ├── config/           # Configurações da aplicação
│   │   ├── controllers/      # Camada HTTP (entrada da API)
│   │   ├── core/             # Domínio da aplicação
│   │   │   ├── entities/     # Entidades de domínio
│   │   │   ├── interfaces/   # Contratos e abstrações
│   │   │   ├── types/        # Tipos derivados
│   │   │   └── usecases/     # Regras de negócio
│   │   ├── database/         # Configuração e acesso ao banco de dados
│   │   ├── middlewares/      # Middlewares do Express
│   │   ├── repositories/    # Implementações de acesso a dados
│   │   ├── routes/           # Definição de rotas
│   │   ├── services/         # Serviços auxiliares
│   │   ├── utils/            # Utilidades compartilhadas
│   │   └── validators/       # Validações e schemas
│   ├── server.ts             # Ponto de entrada da aplicação
│   ├── package.json
│   ├── tsconfig.json
│   └── .gitignore
├── README.md
├── CONTRIBUTING.md
├── DEVELOPMENT_STATUS.md
└── LICENSE
```

---

## 🧠 Princípios de Arquitetura

* Separação entre **domínio** e **infraestrutura**
* Dependência do core apenas de abstrações
* Facilidade para testes e evolução tecnológica
* Planejamento para tarefas assíncronas sem acoplamento

---

## 🚧 Status do Projeto

Detalhes sobre o andamento e próximos passos podem ser encontrados em [`DEVELOPMENT_STATUS.md`](./DEVELOPMENT_STATUS.md).

---

## 🤝 Contribuição

Este projeto é aberto para estudos e contribuições.

Veja as diretrizes em [`CONTRIBUTING.md`](./CONTRIBUTING.md).

---

## 📜 Licença

Este projeto está licenciado sob os termos descritos em [`LICENSE`](./LICENSE).
