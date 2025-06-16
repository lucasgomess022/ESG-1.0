# Sistema ESG Rural

Sistema completo de avaliação ESG (Environmental, Social, and Governance) para propriedades rurais de pecuária bovina.

## 🚀 Deploy Rápido

### Render.com (Recomendado)

1. **Fork este repositório** no GitHub
2. **Acesse [render.com](https://render.com)** e conecte sua conta GitHub
3. **Clique em "New"** → **"Web Service"**
4. **Selecione seu repositório** forkado
5. **Configure:**
   - **Name**: `sistema-esg-rural`
   - **Environment**: `Node`
   - **Build Command**: `npm ci && npm run build`
   - **Start Command**: `npm start`
6. **Adicione um banco PostgreSQL:**
   - Clique em "New" → "PostgreSQL"
   - Name: `esg-database`
7. **Deploy automático!** 🎉

### Outras Plataformas

Para deploy em outras plataformas, consulte o arquivo `deploy-instructions.md`.

## 🛠️ Desenvolvimento Local

```bash
# Clone o repositório
git clone <seu-repositorio>
cd sistema-esg-rural

# Instale dependências
npm install

# Configure variáveis de ambiente
cp .env.example .env
# Edite o arquivo .env com suas configurações

# Inicie em modo desenvolvimento
npm run dev
```

## 📋 Funcionalidades

- ✅ **Questionário ESG Completo** - 50+ perguntas categorizadas
- ✅ **Sistema de Pontuação** - Classificação automática (A, B, C, D, E)
- ✅ **Dashboard Administrativo** - Visualização de resultados
- ✅ **Autenticação Segura** - Sistema de login protegido
- ✅ **Banco de Dados** - PostgreSQL com Drizzle ORM
- ✅ **Interface Responsiva** - Funciona em desktop e mobile
- ✅ **Deploy Automático** - Pronto para produção

## 🏗️ Tecnologias

- **Frontend**: React + TypeScript + Tailwind CSS
- **Backend**: Node.js + Express + TypeScript
- **Banco**: PostgreSQL + Drizzle ORM
- **Build**: Vite + ESBuild
- **Deploy**: Render.com (recomendado)

## 📊 Estrutura do Projeto

```
sistema-esg-rural/
├── client/          # Frontend React
├── server/          # Backend Express
├── shared/          # Schemas compartilhados
├── migrations/      # Migrações do banco
└── deploy-instructions.md
```

## 🔧 Scripts Disponíveis

```bash
npm run dev      # Desenvolvimento
npm run build    # Build para produção
npm start        # Iniciar produção
npm run check    # Verificar TypeScript
npm run db:push  # Atualizar banco
```

## 🌱 Variáveis de Ambiente

| Variável | Descrição | Obrigatória |
|----------|-----------|-------------|
| `DATABASE_URL` | String conexão PostgreSQL | ✅ |
| `SESSION_SECRET` | Chave secreta sessões | ✅ |
| `NODE_ENV` | Ambiente (development/production) | ✅ |
| `PORT` | Porta do servidor | ❌ (padrão: 5000) |

## 📈 Como Usar

1. **Acesse a aplicação** na URL fornecida
2. **Responda o questionário ESG** (50+ perguntas)
3. **Visualize sua classificação** (A-E)
4. **Acesse o dashboard admin** (login necessário)
5. **Analise os resultados** de todas as avaliações

## 🔒 Segurança

- ✅ Autenticação com sessões seguras
- ✅ Validação de dados com Zod
- ✅ Sanitização de inputs
- ✅ Headers de segurança
- ✅ Rate limiting

## 📞 Suporte

Para problemas ou dúvidas:
1. Verifique os logs da aplicação
2. Consulte o arquivo `deploy-instructions.md`
3. Teste localmente com `npm run dev`

## 📄 Licença

MIT License - veja o arquivo LICENSE para detalhes.

---

**Desenvolvido com ❤️ para o agronegócio sustentável**

