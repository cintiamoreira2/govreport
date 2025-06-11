
# 📄 GovReport.NET – Portal de Governança e Divulgação Corporativa

Projeto simulado de um portal usado por empresas listadas na bolsa para envio, armazenamento e consulta pública de documentos regulatórios.

## 🎯 Objetivo

Criar uma aplicação web fullstack com:
- Upload e consulta de documentos oficiais (PDFs)
- Área interna de envio
- Área pública de consulta
- API REST em .NET Core
- Frontend com AngularJS
- Deploy com Docker

## 🧱 Tech Stack

| Camada     | Tecnologia                              |
|------------|------------------------------------------|
| Backend    | ASP.NET Core (.NET 6)                    |
| Frontend   | AngularJS + HTML/CSS + Bootstrap         |
| Banco      | Simulação em memória (DocumentStore.cs) |
| Deploy     | Docker + Docker Compose                  |
| Outros     | NGINX, Git                               |

## 📸 Funcionalidades

✅ Área autenticada (simulada) para envio de documentos  
✅ Upload de arquivos PDF com título, tipo e descrição  
✅ Armazenamento local em `wwwroot/uploads`  
✅ Consulta pública com filtros e download direto  
✅ Containerização com Docker

## 🚀 Como rodar o projeto

> Pré-requisitos: [Docker + Docker Compose](https://docs.docker.com/compose/install/)

### 1. Clone este repositório

```bash
git clone https://github.com/seu-usuario/govreport.git
cd govreport
```

### 2. Suba os containers

```bash
docker-compose up --build
```

### 3. Acesse no navegador

- 🔒 Upload (intranet simulada): `http://localhost:8080/upload.html`  
- 🌐 Consulta pública: `http://localhost:8080/public.html`  
- 🔧 API REST: `http://localhost:5000/api/documentos`  

## 🗃️ Estrutura de Pastas

```
govreport/
├── backend/               # Projeto ASP.NET Core Web API
├── frontend/              # Páginas AngularJS + Bootstrap
├── Dockerfile.backend     # Dockerfile do backend
├── Dockerfile.frontend    # Dockerfile do frontend
├── docker-compose.yml     # Orquestração dos serviços
└── README.md              # Este arquivo
```

## 📌 Observações

- O backend armazena os arquivos localmente em volume Docker (`uploads-data`)
- Para ambiente real, é possível integrar:
  - Banco SQL Server
  - Autenticação JWT
  - Azure Blob Storage ou AWS S3
  - Kafka ou TIBCO para mensageria
  - Pipeline CI/CD com Azure DevOps ou GitHub Actions

## 💼 Vitrine (exemplo de portfólio)

Este projeto simula o ambiente e responsabilidades de áreas de Governança de Empresas Listadas, semelhante às da B3, com foco em:

- Entendimento de domínio regulatório
- Boas práticas de arquitetura
- Capacidade de entrega de soluções fullstack
- Uso de tecnologias relevantes do mercado financeiro e enterprise

## 🙋‍♀️ Autor(a)

**[Seu Nome Aqui]**  
📧 seuemail@exemplo.com  
🔗 [linkedin.com/in/seunome](https://linkedin.com/in/seunome)
