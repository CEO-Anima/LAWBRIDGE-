# LawBridge - Sistema de Prática Jurídica Digital

**LawBridge — onde a prática jurídica ganha vida.**

Sistema completo de simulação de processos judiciais para o Núcleo de Prática Jurídica (NPJ), desenvolvido para facilitar o ensino prático do Direito.

## 📋 Sobre o Projeto

O LawBridge é uma interface simplificada do PJe (Processo Judicial Eletrônico) desenvolvida especificamente para fins educacionais. O sistema permite que professores criem casos judiciais simulados e alunos pratiquem a elaboração de petições e acompanhamento de processos.

## ✨ Funcionalidades Principais

### Para Professores (Juiz)
- 📊 Dashboard com métricas de casos ativos, pendentes e concluídos
- ➕ Criação de casos com upload de documentos iniciais
- 📁 Gerenciamento completo de processos
- 👥 Designação de alunos para acusação e defesa
- 📝 Visualização e anotações em documentos
- ⚖️ Publicação de sentenças

### Para Alunos
- 📂 Visualização de processos designados
- 📄 Envio de petições em PDF
- 📎 Upload de documentos e provas
- 🔔 Notificações de movimentações
- 💬 Mensagens com o professor

### Funcionalidades Gerais
- 🔐 Autenticação com JWT
- 📱 Interface responsiva (desktop-first)
- 🎨 Design profissional inspirado no PJe
- 📋 Timeline de movimentações processuais
- 🔍 PDF Viewer integrado
- 🏷️ Sistema de tags e status
- 🔒 Controle de documentos sigilosos

## 🚀 Como Rodar o Projeto

### Pré-requisitos
- Node.js (versão 18 ou superior)
- npm ou bun

### Instalação

```bash
# Clone o repositório
git clone <YOUR_GIT_URL>

# Entre no diretório
cd simuljus

# Instale as dependências
npm install

# Inicie o servidor de desenvolvimento
npm run dev
```

O projeto estará disponível em `http://localhost:8080`

## 👥 Usuários de Teste

O sistema vem com 3 usuários pré-configurados para testes:

### Professor (Juiz)
- **Email:** egidio.npj@gmail.com
- **Senha:** egidio369
- **Função:** Criar casos, designar alunos, adicionar anotações, publicar sentenças

### Aluno 1 (Acusação)
- **Email:** matheusferreirags10@gmail.com
- **Senha:** 292318anima
- **Função:** Enviar petições e documentos da acusação

### Aluno 2 (Defesa)
- **Email:** marialuiza123@gmail.com
- **Senha:** 123luiza
- **Função:** Enviar petições e documentos da defesa

## 🛠️ Tecnologias Utilizadas

- **Frontend:** React 18 + TypeScript
- **Build Tool:** Vite
- **Estilização:** TailwindCSS + shadcn/ui
- **Roteamento:** React Router v6
- **Estado:** Zustand (com persistência)
- **Upload:** React Dropzone
- **PDF Viewer:** React-PDF (PDF.js)
- **Formulários:** React Hook Form + Zod
- **Ícones:** Lucide React
- **Notificações:** Sonner

## 📁 Estrutura do Projeto

```
src/
├── components/
│   ├── layout/           # Layout components (Sidebar, Header)
│   ├── shared/           # Shared components (FileUploader, PDFViewer)
│   └── ui/              # shadcn/ui components
├── pages/               # Page components
│   ├── Login.tsx
│   ├── Dashboard.tsx
│   ├── CreateCase.tsx
│   ├── Cases.tsx
│   └── NotFound.tsx
├── store/              # Zustand stores
│   ├── authStore.ts
│   └── caseStore.ts
├── lib/                # Utilities
└── hooks/              # Custom React hooks
```

## 🎨 Design System

O SimulJus utiliza uma paleta de cores profissional inspirada no sistema judiciário brasileiro:

- **Primary (Azul Judicial):** `hsl(215, 85%, 35%)`
- **Success (Verde):** Para casos concluídos
- **Warning (Laranja):** Para casos pendentes
- **Muted:** Para elementos secundários
- **Sidebar:** Fundo escuro profissional

Todos os tokens de cor estão definidos em `src/index.css` e podem ser facilmente personalizados.

## 📝 Mock Data

O sistema vem com dados simulados (mock) para facilitar o desenvolvimento e testes:

- 1 caso de exemplo: NPJ-2025-0001 (Ação Penal - Homicídio Qualificado)
- 3 usuários com diferentes perfis
- Timeline com movimentações processuais

## 🔜 Próximas Funcionalidades

- [ ] Visualizador de PDF com anotações
- [ ] Sistema de notificações em tempo real
- [ ] Chat entre professor e alunos
- [ ] Exportação de processos em PDF
- [ ] Relatórios e estatísticas
- [ ] Upload em lote com preview
- [ ] Assinaturas digitais simuladas
- [ ] Integração com backend real

## 🤝 Contribuindo

Este é um projeto educacional desenvolvido para o NPJ. Contribuições são bem-vindas!

## 📄 Licença

Este projeto é de uso pessoal.

---

