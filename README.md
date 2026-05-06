# ⚙️ Gallery Plus — Backend

API REST desenvolvida com **Fastify**, **Node.js** e **TypeScript**, responsável pela camada de dados do app Gallery Plus.

Construída com foco em **performance**, **upload de arquivos** e **relacionamento N:N** entre fotos e álbuns — servindo como base real para o front-end em produção.

🔗 **Deploy ativo no Render**

---

## 🚀 Tecnologias

- Node.js
- Fastify
- TypeScript
- Zod (validação de dados)
- `@fastify/multipart` (upload de arquivos)
- `@fastify/static` (servir arquivos estáticos)
- `@fastify/cors` (controle de origem)
- tsup (build)
- tsx (desenvolvimento)

---

## ✅ Funcionalidades

### 📷 Fotos
- Upload de imagens via multipart
- Listagem de todas as fotos
- Detalhes de uma foto específica
- Associação de uma foto a múltiplos álbuns

### 🗂️ Álbuns
- Criação de álbuns
- Listagem de álbuns
- Visualização de fotos de um álbum
- Associação de um álbum a múltiplas fotos

### 🔗 Relacionamento N:N
- Uma foto pode pertencer a múltiplos álbuns
- Um álbum pode conter múltiplas fotos

---

## 🧱 Arquitetura

A API foi estruturada com separação clara de responsabilidades:

- **Routes** — define os endpoints e delega para os handlers
- **Handlers** — contém a lógica de cada operação
- **Zod Schemas** — valida os dados de entrada em cada rota
- **Static** — serve as imagens armazenadas localmente

---

## ▶️ Como executar

```bash
# Instalar dependências
npm install

# Modo desenvolvimento
npm run dev

# Build para produção
npm run build

# Rodar em produção
npm start
```

---

## 🎯 Próximas implementações

- [ ] Autenticação de usuários
- [ ] Associação de fotos/álbuns ao usuário autenticado
- [ ] Migração para banco de dados relacional

---

## 👨‍💻 Autor

Desenvolvido por **Junior Bonini** como parte do projeto Gallery Plus — portfólio profissional com foco em integração Full Stack real.
