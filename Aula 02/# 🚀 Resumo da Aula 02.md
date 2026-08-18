# 🚀 Aula 02 - Configuração do Ambiente de Desenvolvimento

## 📚 Sumário

- 🔄 Introdução ao Versionamento
- 🏷️ Versionamento Semântico (SemVer)
- 🌿 Git e Controle de Versão
- 🔖 Tags, Branches e Boas Práticas no Git
- 💻 IDE e Visual Studio Code
- 🟢 Node.js e NPM
- ⚛️ Criação de Projetos React
- ☁️ Deploy e Hospedagem com Vercel
- 📝 Atividade Prática

---

# 🔄 Introdução ao Versionamento

Versionamento é o processo de atribuir identificadores únicos para diferentes versões de um software.

## ✅ Benefícios

- 📜 Histórico completo das alterações
- 👤 Registro de autoria
- 🤝 Colaboração entre desenvolvedores
- ⏪ Recuperação de versões anteriores
- 🔎 Auditoria e rastreabilidade

## 📊 Versionamento x Backup

| 🔄 Versionamento | 💾 Backup |
|-----------------|----------|
| Histórico completo | Cópia pontual |
| Rastreabilidade | Sem autoria |
| Colaboração simultânea | Arquivos duplicados |
| Reversão granular | Restauração total |

---

# 😱 O Caos Sem Versionamento

- 💾 `versao_final_agora_sim2.zip`
- 🔥 Código perdido
- ⚠️ Conflitos entre desenvolvedores
- 🔍 Sem histórico de alterações

---

# 🏷️ Versionamento Semântico (SemVer)

O SemVer utiliza o padrão:

```txt
MAJOR.MINOR.PATCH
```

## 📌 Estrutura

### 🔴 MAJOR (2.0.0)

Mudanças incompatíveis com versões anteriores.

### 🟡 MINOR (1.1.0)

Novas funcionalidades compatíveis.

### 🟢 PATCH (1.0.1)

Correções de bugs sem quebrar funcionalidades.

---

## 📖 Exemplos

| Versão | Descrição |
|---------|------------|
| 1.0.0 | Primeira versão estável |
| 1.1.0 | Nova funcionalidade |
| 1.1.1 | Correção de bug |
| 2.0.0 | Alteração incompatível |

---

## 🔧 Tipos de Alterações

- 🐞 Bug Fix
- ✨ New Feature
- 🚀 Feature Enhancement
- ♻️ Refactoring
- ⚡ Performance
- 🔒 Security Patch
- 📦 Dependency Update
- ✅ Adding Tests

---

# 🌿 Git

Git é um sistema de controle de versão distribuído.

## ✅ O Git Permite

- 💾 Salvar versões do projeto
- 📜 Manter histórico de alterações
- 🔄 Sincronizar com GitHub
- 👥 Trabalhar em equipe
- ♻️ Restaurar versões antigas

---

# ⚙️ Instalando o Git

## 1️⃣ Baixar

🔗 https://git-scm.com/downloads

## 2️⃣ Verificar Instalação

```bash
git --version
```

## 3️⃣ Configurar Usuário

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

---

# 🔖 Tags no Git

Tags servem para marcar versões importantes.

## Criar uma Tag

```bash
git tag 1.0.0
```

## Listar Tags

```bash
git tag
```

## Enviar Tag para o GitHub

```bash
git push origin 1.0.0
```

---

# ✅ Boas Práticas com Git

## 📝 Commits

- Pequenos e frequentes
- Mensagens claras

Exemplo:

```bash
git commit -m "Corrige validação do formulário"
```

## 🌿 Branches

- `main` sempre estável
- Novas funcionalidades em branches separadas

```bash
git checkout -b feature/login
```

## ✅ Testes

- Testar antes do merge
- Automatizar quando possível

---

# 💻 IDE e VS Code

## O que é uma IDE?

IDE (*Integrated Development Environment*) é um ambiente que reúne ferramentas para:

- ✍️ Escrever código
- 🐞 Depurar
- ▶️ Executar
- ✅ Testar aplicações

## Visual Studio Code

- 🆓 Gratuito
- 🔌 Extensível
- ⚡ Leve
- 🌎 Multiplataforma

---

# 🟢 Node.js

Node.js permite executar JavaScript fora do navegador.

## ✅ Benefícios

- 🚀 Alta performance
- 🌐 Backend com JavaScript
- 🔄 Integração entre Front-end e Back-end

---

## 📥 Instalação

🔗 https://nodejs.org

Verifique a instalação:

```bash
node --version
```

---

# 📦 NPM (Node Package Manager)

NPM é instalado automaticamente junto com o Node.js.

## ✅ Funções

- 📥 Instalar bibliotecas
- 🔄 Atualizar dependências
- 🗑️ Remover pacotes
- 📋 Gerenciar projetos

Verificar versão:

```bash
npm --version
```

---

# 📄 package.json

Arquivo responsável por armazenar:

- Dependências
- Scripts
- Configurações do projeto

Exemplo:

```json
{
  "name": "meu-projeto",
  "version": "1.0.0"
}
```

---

# ⚛️ Criando um Projeto React

## 1️⃣ Criar Projeto

```bash
npx create-react-app meu-projeto-react
```

## 2️⃣ Entrar na Pasta

```bash
cd meu-projeto-react
```

## 3️⃣ Abrir no VS Code

```bash
code .
```

## 4️⃣ Executar Projeto

```bash
npm start
```

---

# 📁 Estrutura do Projeto React

```txt
meu-projeto-react/
│
├── node_modules/
├── public/
├── src/
├── package.json
├── package-lock.json
└── .gitignore
```

## 📂 Principais Pastas

### 📦 node_modules

Contém todas as bibliotecas instaladas.

### 🌍 public

Contém:

- HTML
- Imagens
- JSON
- Arquivos estáticos

### ⚛️ src

Contém o código-fonte da aplicação.

---

# 🧩 Arquivos Principais

## index.js

Ponto de entrada da aplicação React.

```javascript
ReactDOM.createRoot(
  document.getElementById("root")
);
```

## App.js

Componente principal da aplicação.

```javascript
function App() {
  return <h1>Olá React!</h1>;
}

export default App;
```

## 🎨 App.css

Estilos do componente App.

## 🌐 index.css

Estilos globais da aplicação.

---

# ☁️ Deploy

Deploy é o processo de disponibilizar uma aplicação para os usuários finais.

## ✅ Etapas

1. 🏗️ Build
2. ⚙️ Configuração
3. ✅ Testes
4. 🚀 Publicação

---

# ☁️ Vercel

Plataforma moderna para hospedagem e deploy de aplicações web.

## 🚀 Recursos

- 🔗 Integração com GitHub
- 🚀 Deploy Automático
- 🌎 CDN Global
- 🔄 Rollback de versões
- ⚡ Alta Performance
- 📈 Escalabilidade automática

---

# 🔄 Fluxo GitHub + Vercel

```txt
⚛️ React
      ↓
🌿 Git
      ↓
🐙 GitHub
      ↓
☁️ Vercel
      ↓
🌐 URL Pública
```

---

# 📝 Atividade Prática

## 🎯 Desafio

1. ⚛️ Criar uma aplicação React
2. 🌿 Inicializar um repositório Git
3. 📤 Publicar no GitHub
4. ☁️ Conectar à Vercel
5. 🚀 Publicar a aplicação online

### ✅ Resultado Esperado

- ✅ Aplicação React funcionando
- ✅ Código disponível no GitHub
- ✅ Deploy realizado na Vercel
- ✅ URL pública acessível

---

# 🎯 Resumo Final

- 🔄 Versionamento organiza o desenvolvimento.
- 🌿 Git controla alterações do projeto.
- 🏷️ SemVer padroniza versões.
- 💻 VS Code é a IDE utilizada.
- 🟢 Node.js executa JavaScript no servidor.
- 📦 NPM gerencia dependências.
- ⚛️ React facilita a criação de interfaces modernas.
- ☁️ Vercel simplifica deploy e hospedagem.
- 🚀 GitHub + Vercel automatizam a publicação de aplicações.
